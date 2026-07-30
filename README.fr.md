<p align="center">
  <img src="brand/dubsar-readme-header-fr.svg" alt="DUBSAR — Gouverner le passage de l’intention à la preuve. Conserver l’autorité humaine." width="100%" />
</p>

# DUBSAR

**Auditez vos automatisations. Gouvernez ce qui agit.**

DUBSAR relie les faits, les décisions et les preuves de vos workflows. Le
système rend les incohérences visibles, conserve les limites de couverture et
remet la validation au responsable humain désigné.

La direction publique actuelle repose sur deux surfaces :

1. un portail d’audit automatisé, en construction et bientôt disponible ;
2. un Audit professionnel DUBSAR borné, disponible sur demande.

[Découvrir l’audit](https://dubsar.ai/fr/audit) ·
[État actuel](STATUS.md) ·
[English version](README.md)

---

## Deux surfaces, une même méthode

| Surface | Usage | Statut actuel |
|---|---|---|
| **Portail d’audit automatisé** | Examiner un périmètre d’automatisations, relier les événements disponibles et préparer un rapport validable | En construction et en validation ; bientôt disponible |
| **Audit professionnel DUBSAR** | Examiner un projet ou une automatisation sous mandat, avec sources autorisées et revue humaine | Disponible sur demande |

Le portail est destiné à préparer un premier résultat structuré. L’audit
professionnel ajoute un mandat convenu, une analyse opérateur et une revue
humaine. Aucune de ces surfaces n’est destinée à produire automatiquement un
verdict juridique ou réglementaire.

### Portail d’audit automatisé

La page publique de l’audit constitue le point d’entrée produit actuel. Le
portail lui-même n’est pas encore accessible au public.

Le parcours visé est le suivant :

1. définir les automatisations, la période et les sources autorisées ;
2. relier les événements disponibles sans inventer de causalité ;
3. signaler les incohérences, incertitudes et informations manquantes ;
4. faire classer les constats par le responsable désigné ;
5. produire un rapport où preuves, limites et validations restent reliées.

L’autonomie ne signifie ni décision automatique, ni certification, ni
suppression de la responsabilité humaine.

[Découvrir l’audit automatisé](https://dubsar.ai/fr/audit)

### Audit professionnel DUBSAR

L’Audit professionnel DUBSAR est une intervention bornée, opérée par Sofiane
avec DUBSAR. Ses principaux mandats sont la préparation au lancement et la
gouvernance des agents.

Chaque intervention commence par un accord explicite sur le périmètre, les
sources autorisées, les permissions, les limites d’accès, la conservation, le
calendrier, le prix et les livrables. La lecture seule est la règle par défaut.
Les faits, inférences, contradictions, limites et décisions humaines restent
distincts.

[Comprendre la méthode](AUDIT.fr.md) ·
[Demander un audit](https://dubsar.ai/fr/audit) ·
[Contact](mailto:contact@dubsar.ai)

---

## Doctrine commune

Toutes les surfaces actuelles de DUBSAR suivent les mêmes principes :

- seules les sources autorisées sont examinées ;
- une affirmation n’est jamais traitée comme une preuve ;
- les faits et les inférences restent séparés ;
- la provenance et la version des preuves sont conservées ;
- les contradictions et les limites restent visibles ;
- une source absente devient une limite, pas une conformité implicite ;
- la lecture seule est la règle par défaut ;
- aucun agent ne peut approuver seul son propre travail ;
- les décisions protégées restent sous autorité humaine.

**Les systèmes analysent et appliquent des règles déclarées. DUBSAR conserve et
vérifie. L’humain autorise et décide.**

```text
Sources autorisées
    ↓
Audit DUBSAR
    ↓
Preuves, incohérences et limites
    ↓
Validation humaine
    ↓
Rapport validable
```

Une gouvernance continue ou des composants installés pourront éventuellement
être étudiés plus tard dans un périmètre distinct. Leur architecture,
distribution, support et licence restent indécis et ne sont pas promis par
l’audit initial.

---

## Skills publics

Le dépôt distinct
[dubsar-agent-skills](https://github.com/kotnisofiane-bit/dubsar-agent-skills)
publie sous licence MIT une doctrine et des assistants locaux bornés pour les
travaux d’audit et de gouvernance.

Ces skills constituent une ressource publique complémentaire. Ils ne sont
**ni** le produit DUBSAR, **ni** le Portail, le Core privé ou un runtime ; ils
ne donnent accès à aucun service privé et ne constituent pas une
installation prise en charge de DUBSAR. Leur licence s’applique uniquement à
ce dépôt.

---

## Travaux antérieurs sur les agents de code

Les premières expérimentations DUBSAR ont étudié la gouvernance de projets
assistés par des agents de code, avec notamment un paquet de préparation pour
Claude Code. Ces travaux ont nourri la doctrine actuelle sur la preuve et
l’autorité humaine, mais ne constituent plus une surface commerciale actuelle
ni une bêta publique ou privée active.

L’ancienne surface de Marketplace a été retirée de l’arbre actif. Ce dépôt ne
propose aucun plugin public, runtime, accès bêta ou parcours d’installation
pris en charge. Les décisions produit futures seront documentées lorsqu’elles
seront définies et validées.

---

## AI Act

DUBSAR peut aider à structurer des éléments utiles à une préparation
documentaire liée à l’AI Act :

- inventaire des systèmes, agents, responsables et finalités ;
- traçabilité des sources, versions, décisions et validations ;
- supervision humaine explicite ;
- limites, incertitudes et informations manquantes ;
- registres de preuves et de contradictions.

DUBSAR ne fournit aucun conseil juridique, ne délivre aucune certification et
ne produit aucun verdict automatique de conformité.

---

## Frontière publique et privée

Ce dépôt constitue la frontière documentaire publique de DUBSAR. Il ne s’agit
pas d’une distribution logicielle publique.

Il peut contenir :

- la doctrine et l’architecture publiques ;
- des exemples et diagrammes bornés ;
- les informations publiques de sécurité, confidentialité et état de
  distribution ;
- des archives historiques non exécutables.

Il ne publie pas :

- le Portail ou toute autre implémentation produit privée ;
- le Core propriétaire ;
- tout composant DUBSAR actuellement installable ;
- les politiques ou journaux internes ;
- les données de clients ou de testeurs ;
- les secrets, jetons ou éléments de confiance ;
- les détails privés du Backend.

Aucune licence logicielle publique n’est actuellement choisie ou accordée par
ce dépôt. Les licences futures seront décidées séparément pour chaque composant
avant toute distribution. Les éléments tiers restent soumis à leurs propres
licences et notices. Voir [Droits et statut des licences](RIGHTS.md).

---

## Documentation

### Comprendre DUBSAR

1. [Pourquoi DUBSAR ?](WHY_DUBSAR.md)
2. [Audit DUBSAR](AUDIT.fr.md)
3. [Produit et surfaces](PRODUCT_SURFACES.md)
4. [État actuel](STATUS.md)
5. [Architecture](ARCHITECTURE.md)
6. [FAQ](FAQ.md)
7. [Feuille de route](ROADMAP.md)

### Distribution et confiance

- [Droits et statut des licences](RIGHTS.md)
- [Installation](INSTALLATION.md)
- [Historique Marketplace et état de distribution](MARKETPLACE.md)
- [Sécurité](SECURITY.md)
- [Confidentialité](PRIVACY.md)
- [Intégrité et provenance](INTEGRITY.md)

---

## Créé par

Créé par [**Sofiane Kotni**](https://dubsar.ai/fr/sofiane-kotni/), créateur de
DUBSAR et auteur de *Digital Trust*.

[Site DUBSAR](https://dubsar.ai/fr/) ·
[LinkedIn](https://www.linkedin.com/in/sofiane-kotni/) ·
[GitHub](https://github.com/kotnisofiane-bit) ·
[Skills publics](https://github.com/kotnisofiane-bit/dubsar-agent-skills) ·
[Digital Trust — français](https://www.amazon.fr/dp/B0H739BFJP) ·
[Digital Trust — anglais](https://www.amazon.fr/dp/B0GZ4RH1KX) ·
[Page auteur Amazon](https://www.amazon.fr/stores/Sofiane-KOTNI/author/B0H6NBHZTC) ·
[Contact](mailto:contact@dubsar.ai)
