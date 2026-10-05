# DUBSAR

**Un control plane pour du travail agentique durable et gouverné.**

Les agents réalisent le travail. DUBSAR conserve l’état durable des missions,
les preuves, l’état opérationnel, le jugement borné et l’autorité explicite
hors de l’agent lui-même. Le travail doit survivre à une fin de session, à un
crash ou à un changement d’agent ou de fournisseur de modèle.

> Le logiciel porte la réalité.
> Le modèle porte le jugement.
> Les humains conservent l’autorité sur les effets conséquents.

Ce dépôt est le **point d’entrée public canonique** de DUBSAR. Il reste une
racine documentaire technique, sans code applicatif ni version Personal
publiquement installable. Le développement est actif ; des tests de
composants ne constituent ni un produit intégré ni une disponibilité générale.

[État actuel](STATUS.md) · [Architecture](ARCHITECTURE.md) ·
[English version](README.md)

## Pourquoi DUBSAR existe

Une session d’agent peut produire un résultat utile tout en perdant la mission,
ses contraintes, les preuves d’une décision ou l’autorité nécessaire pour agir.
L’historique de conversation et les logs d’exécution ne suffisent pas à
conserver ce travail.

DUBSAR sépare ce qui est connu, proposé, autorisé et réellement observé.
Réussite d’exécution, réussite de mission et preuve restent distinctes.
Voir [Pourquoi DUBSAR ?](WHY_DUBSAR.md) et
[Pourquoi pas seulement des agents ?](WHY_NOT_JUST_AGENTS.md).

## Une architecture, deux environnements

Ce schéma répartit les responsabilités ; il ne déclare pas tous les parcours
déjà intégrés :

```text
Faits / État / Preuves
        ↓
Logiciel déterministe
        ↓
Judgment borné
        ↓
Autorité explicite
        ↓
Agents / Automatisation / Outils
```

Les agents exécutent le travail. Le logiciel déterministe possède l’état
canonique, les permissions et les enregistrements de preuve. Judgment propose
le prochain mouvement cognitif justifié ; il n’a aucune autorité. Les
politiques et Human Gates restent autoritaires pour les effets conséquents.
Les observations d’exécution passent par une validation logicielle avant
toute mise à jour de l’état canonique.

### DUBSAR Personal

Personal est la première expression produit du système : une expérience
Desktop pour les missions durables. Son architecture cible actuelle est :

```text
Desktop
├─ My Work / missions durables
├─ Agents / Hermes
├─ Memory
├─ Automation
├─ Tool Layer / Connectors
├─ Operational Context / Evidence
├─ Judgment
├─ Trace Canvas
└─ Human Gates
```

L’utilisateur doit pouvoir changer d’agent ou de fournisseur de modèle sans
perdre le travail lui-même. My Work, Memory et les traces doivent se rapporter
à la même mission et au même état de progression.

**Statut : intégration active / développement technique.** Desktop, Trace
Canvas, Judgment local et la continuité d’une mission entre toutes les vues
restent en intégration. Cela n’annonce ni bêta publique, ni plateformes prises
en charge, ni support commercial.

### DUBSAR Control Plane

Control Plane applique le même modèle d’état, de preuves et d’autorité aux
workloads agentiques plus lourds ou organisationnels :

```text
Décision humaine / Core
→ Autorisation signée / Task Lease
→ Admission runtime
→ Handoff durable
→ Workload / sandbox
→ Egress médié
→ Gateway / Broker
→ Evidence / Operational Context
```

L’agent ne possède pas les identifiants du fournisseur. L’autorisation est un
objet validé, pas une instruction dans un prompt. L’admission et les décisions
de replay doivent être déterministes. Un crash ne doit pas créer
silencieusement une seconde exécution. L’egress peut être médié ; l’agent ne
peut pas s’approuver lui-même.

Ces frontières décrivent l’architecture et les exigences d’intégration.
Elles ne déclarent pas toute la stack intégrée live ou qualifiée dans chaque
runtime réel. Voir [ARCHITECTURE.md](ARCHITECTURE.md).

## Judgment

Judgment est un policy/controller probabiliste borné. Il choisit un prochain
mouvement cognitif dans un ensemble fermé, par exemple `consult`, `conclude`,
`clarify`, `revise` ou `stop`. Ce n’est pas un super-agent orchestrateur.
Le logiciel valide la proposition puis exécute uniquement les actions
autorisées.

Judgment ne peut ni créer une permission ou une preuve, ni déclarer une source
fraîche, ni terminer une mission sans support, ni se donner une autorité, ni
affirmer qu’une action a réellement réussi. Proposer `conclude` ne clôture pas
la mission. Qwen est le candidat local actuel, pas une dépendance identitaire
de l’architecture.

## Ce qui existe aujourd’hui

Le développement dispose de composants fonctionnels pour l’état durable du
travail là où il est pris en charge, les contrats et validateurs déterministes,
les frontières de preuve et les patterns Human Gate. L’automatisation et les
contrats AgentContext / Judgment font partie du travail technique.
L’intégration reste active.

[STATUS.md](STATUS.md) distingue composants acquis, intégration active et
capacités non revendiquées. Il sépare aussi l’état technique rapporté par le
projet de ce qu’un lecteur peut inspecter publiquement. Un test ne devient pas
une annonce de disponibilité produit.

## Composants techniques

- [DUBSAR Memory](https://github.com/kotnisofiane-bit/dubsar-memory) : preview
  technique publique d’un moteur déterministe de mémoire projet, d’une CLI
  et d’un Workbench en lecture seule. Son README définit son périmètre et sa
  licence. Ce n’est ni Personal unifié ni une distribution de Control Plane.
- Les autres dépôts seront référencés lorsque leur code et leur périmètre
  publics seront disponibles. `dubsar-contracts` n’est pas présenté comme
  public.

Cette racine reste canonique pour le projet. Les anciennes phases audit,
skills, Marketplace et Scribe sont indexées dans [LEGACY.md](LEGACY.md) ;
elles ne définissent pas la disponibilité actuelle.

## Documentation

- [Surfaces produit](PRODUCT_SURFACES.md) : Personal et Control Plane.
- [Philosophie](DESIGN_PHILOSOPHY.md) et [Principes](PRINCIPLES.md) :
  état, jugement et autorité.
- [Roadmap](ROADMAP.md) : priorités d’intégration sans promesse de sortie.
- [FAQ](FAQ.md), [Installation](INSTALLATION.md), [Sécurité](SECURITY.md),
  [Confidentialité](PRIVACY.md) et [Droits](RIGHTS.md) : frontières publiques.

Créé par **Sofiane Kotni**.
