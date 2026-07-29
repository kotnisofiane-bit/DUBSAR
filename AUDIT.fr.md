# Audit DUBSAR

L’Audit DUBSAR est le point d’entrée principal du produit dans le portail.

Sa première cible est un **audit borné de cohérence des automatisations** :
connecter ou importer des preuves autorisées issues d’un système
d’automatisation et d’un système métier, détecter des incohérences précises,
faire examiner chaque constat proposé par un humain, puis produire un rapport
relié aux preuves.

Ce n’est ni une certification juridique, ni un verdict générique sur l’IA, ni
la promesse de reconstruire automatiquement tous les processus métier.

## Premier profil d’audit : cohérence des automatisations

Le premier profil de travail utilise des exports bornés de n8n et HubSpot. Il
pose trois questions :

1. La même conséquence métier a-t-elle été exécutée plusieurs fois sans
   frontière d’idempotence attribuable ?
2. Une action a-t-elle été exécutée alors que l’état métier disponible indiquait
   qu’elle ne devait pas l’être ?
3. Les sources connectées permettent-elles d’établir la version du workflow, la
   règle active et la validation humaine attendue pour une action sensible ?

Le troisième contrôle est volontairement borné. Lorsque la preuve manque,
DUBSAR doit indiquer **« aucune preuve trouvée dans les sources connectées »**,
et non affirmer que l’événement ou la validation n’a jamais existé.

Ces contrôles produisent des constats candidats dans un périmètre de preuves
déclaré. Ils ne prouvent ni la causalité, ni l’exhaustivité, ni la conformité
réglementaire.

## Parcours autonome visé

Le parcours prévu dans le portail est le suivant :

```text
Créer ou ouvrir un espace d’audit
    ↓
Autoriser et fournir des sources bornées
    ↓
Figer l’instantané de preuves et sa couverture
    ↓
Exécuter les contrôles déterministes
    ↓
Expliquer les constats candidats avec l’assistance d’agents
    ↓
Revue humaine : vrai, faux ou incertain
    ↓
Générer le rapport relié aux preuves
```

La revue humaine fait partie du produit ; ce n’est pas un traitement
d’exception. Un modèle peut expliquer, résumer ou proposer une classification,
mais il ne peut pas promouvoir sa propre sortie en vérité vérifiée ni créer un
Human GO.

## Limite de validation actuelle

L’évaluateur de cohérence des automatisations a été exercé sur des jeux de
données synthétiques, et un parcours d’audit au niveau API a été enregistré
dans un déploiement contrôlé.

Le parcours complet dans le navigateur n’a **pas encore été prouvé de bout en
bout comme le ferait un utilisateur normal**. Les preuves actuelles
n’établissent donc pas encore un portail autonome disponible à tous, depuis la
connexion et l’import jusqu’à la revue, au rechargement et à l’export du rapport.

Tant que cette preuve n’existe pas :

- le portail reste en validation interne avec un accès contrôlé ;
- une preuve au niveau API ne doit pas être présentée comme un E2E d’interface ;
- zéro constat signifie « aucun constat détecté dans le périmètre borné », et
  non « l’automatisation est conforme » ;
- une source absente ou incomplète reste visible et peut rendre un contrôle non
  évaluable.

Consultez [l’état actuel](STATUS.md) pour connaître la frontière produit la plus
récente.

## Contenu prévu du rapport

Lorsque le parcours portail sera validé, le rapport devra contenir :

- la question d’audit, le mandat et le périmètre borné ;
- les sources, versions, empreintes et limites de couverture ;
- les constats candidats reliés à leurs références de preuve ;
- les faits observés séparés des éléments dérivés ou inférés ;
- les incertitudes, preuves manquantes et sources indisponibles ;
- la décision humaine sur chaque constat proposé ;
- les actions de suivi prioritaires ;
- un identifiant de rapport reproductible et un registre de preuves.

Le rapport ne doit jamais laisser entendre que les sources connectées étaient
complètes si leur couverture n’a pas réellement été établie.

## Frontières de sécurité et d’autorité

- La collecte en lecture seule est la règle par défaut pour un audit.
- Le site commercial public ne demande aucun identifiant de connecteur, jeton
  ou archive de code source.
- L’accès aux sources doit être explicite, borné et attribuable.
- Aucun ticket, aucune correction, aucun message et aucune mutation externe ne
  sont créés par défaut.
- Une source indisponible est signalée comme une limite ; elle n’est jamais
  silencieusement considérée conforme ou non conforme.
- Les résultats déterministes, les explications des agents et les décisions
  humaines restent des enregistrements distincts.
- Le client reste responsable des décisions métier et de remédiation.

Les flux de données du portail, la conservation, la suppression, les
sous-traitants et l’authentification devront être documentés et validés avant
toute disponibilité générale.

## Après l’audit

L’audit doit pouvoir conduire à une gouvernance continue lorsqu’un client
choisit d’aller plus loin.

Un futur **Node DUBSAR** installé chez le client et administré depuis le desktop
est destiné à relier certains chemins d’exécution d’automatisations et d’agents
au Core DUBSAR privé. Selon le système, cette frontière pourra utiliser une
gateway HTTP contrôlée, une API ou un adaptateur hôte. Elle pourra préparer les
actions sensibles pour une approbation humaine, puis appliquer des décisions de
politique bornées.

Ce chemin de gouvernance installé relève de travaux produit futurs. Il n’est pas
présenté aujourd’hui comme un déploiement prêt pour la production.

Claude Code, Codex, Cursor et les autres adaptateurs pour développeurs restent
une direction secondaire de Developer Labs. Ils ne sont pas nécessaires pour
l’audit portail et ne sont pas présentés comme des intégrations disponibles à
tous.

## Frontière de préparation à l’AI Act

DUBSAR est conçu pour soutenir des travaux concrets de gouvernance : inventaire
des systèmes, traçabilité des preuves, limites documentées et supervision
humaine explicite. Ces capacités peuvent aider une organisation à préparer la
documentation et les contrôles pertinents au regard de l’AI Act européen.

DUBSAR :

- ne détermine pas seul si l’AI Act s’applique à une organisation ou à un
  système ;
- n’attribue pas de classification de risque juridiquement opposable ;
- ne fournit pas de conseil juridique ;
- ne certifie pas la conformité ;
- ne remplace ni le fournisseur, ni le déployeur, ni le conseil juridique, ni
  l’autorité compétente.

## Accompagnement professionnel facultatif

La cible produit est un audit autonome dans le portail, sans obliger Sofiane à
revoir chaque première analyse.

Un accompagnement facultatif pourra être proposé plus tard pour le cadrage,
l’interprétation, la planification des corrections ou l’installation. Il s’agit
d’un service distinct, qui ne doit être présenté ni comme une étape obligatoire
du portail, ni comme disponible tant qu’il n’a pas été annoncé explicitement.

## Suivre la validation

La méthode publique est décrite sur
[dubsar.ai/fr/audit](https://dubsar.ai/fr/audit). L’accès au portail ne sera
présenté comme disponible qu’après validation de ses contrôles d’accès et de son
parcours utilisateur complet.
