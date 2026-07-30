# Audit DUBSAR

Le portail automatisé d’Audit DUBSAR sera bientôt disponible. Il est en cours de
construction et de validation et n’est pas disponible actuellement. Il se
distingue de l’Audit professionnel DUBSAR, disponible sur demande, et de la bêta
privée contrôlée pour Claude Code.

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
bout au niveau requis pour une disponibilité générale ou pour une mise en
production**. Les preuves actuelles n’établissent notamment pas tous les
parcours, de la connexion et l’import jusqu’à la revue, au rechargement et à
l’export du rapport, dans toutes les conditions d’exploitation prises en charge.

Pendant la construction et la validation active :

- le portail reste indisponible au public ;
- une preuve au niveau API ne doit pas être présentée comme un E2E d’interface ;
- zéro constat signifie « aucun constat détecté dans le périmètre borné », et
  non « l’automatisation est conforme » ;
- une source absente ou incomplète reste visible et peut rendre un contrôle non
  évaluable.

Le site marketing public décrit la méthode d’audit prévue ; il ne donne pas
accès au portail.

Consultez [l’état actuel](STATUS.md) pour connaître la frontière produit la plus
récente.

## Contenu prévu du rapport

Le rapport doit contenir :

- la question d’audit, le mandat et le périmètre borné ;
- les enregistrements de provenance des sources, leurs versions, leurs
  empreintes et leurs limites de couverture ;
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
  ou archive de source.
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

Un **Node DUBSAR** installé dans un périmètre distinct et administré depuis le
desktop est destiné à relier certains chemins d’exécution d’automatisations et
d’agents au Core DUBSAR privé. Selon le système, cette frontière pourra utiliser
une gateway HTTP contrôlée, une API ou un adaptateur hôte. Elle pourra préparer
les actions sensibles pour une approbation humaine, puis appliquer des décisions
de politique bornées.

Le Node DUBSAR constitue un chemin de déploiement distinct et n’est pas
disponible de manière générale.

DUBSAR pour Claude Code est une bêta privée contrôlée fonctionnelle en cours de
finalisation. L’accès est sélectif, sur invitation, avec Windows comme première
cible prise en charge. Cette bêta n’est pas nécessaire pour l’audit portail.
Codex et Cursor restent de futures surfaces d’intégration, sans promesse de
disponibilité. L’ancienne surface de Marketplace publique Claude Code a été
retirée de l’arbre actif ; aucun paquet public n’est disponible.

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

## Audit professionnel DUBSAR

Le futur portail autonome est conçu pour ne pas imposer à Sofiane de revoir
chaque première analyse. Pendant sa construction, l’Audit professionnel DUBSAR
reste disponible sur demande pour les organisations qui ont besoin d’un mandat
guidé.

Il s’agit d’une prestation distincte et conduite par un humain pour des travaux
convenus tels que le cadrage, la revue des preuves, l’interprétation, la
planification des corrections ou la préparation d’une installation dans un
périmètre distinct. Le périmètre, les sources autorisées, les permissions, la
conservation, les livrables, le calendrier et le prix sont convenus avant le
démarrage. La collecte en lecture seule reste la règle par défaut et la
prestation ne constitue pas une certification juridique.

Une demande peut être initiée depuis la
[page de l’audit professionnel](https://dubsar.ai/fr/audit) ou le
[profil Malt de Sofiane Kotni](https://www.malt.fr/profile/sofianekotni).

## Suivre la validation

Le portail sera bientôt disponible et reste indisponible pendant sa construction
et sa validation. La méthode publique et la prestation professionnelle sont
décrites sur [dubsar.ai/fr/audit](https://dubsar.ai/fr/audit). L’accès sélectif
à la bêta contrôlée Claude Code est présenté sur
[dubsar.ai/fr/early-access](https://dubsar.ai/fr/early-access).
