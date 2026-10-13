
# TP — Piloter un projet d'infrastructure avec GitHub Projects

**Durée indicative :** 1 heures  
**Organisation :** Individuel ou binôme  
**Outils :** Git, GitHub, GitHub Issues, GitHub Projects

## Objectifs pédagogiques

À l'issue de ce TP, vous devrez être capables de :

- Organiser un projet technique avec GitHub Projects.
- Créer et structurer des issues et des milestones.
- Personnaliser le suivi à l'aide de champs spécifiques.
- Construire différentes vues adaptées aux besoins des utilisateurs.
- Utiliser les regroupements et les agrégations.
- Planifier des interventions avec une roadmap.
- Construire des indicateurs et des graphiques.
- Associer des commits et des Pull Requests aux issues.
- Assurer la traçabilité des interventions techniques.
- Analyser l'avancement d'un projet.

---

## Contexte professionnel

Vous intégrez l'équipe informatique d'une entreprise de 150 collaborateurs répartis sur deux sites.

L'entreprise souhaite moderniser son infrastructure et renforcer sa sécurité informatique.

Plusieurs problèmes ont été identifiés :

- Des serveurs fonctionnent sur des systèmes obsolètes.
- Les sauvegardes ne sont pas régulièrement vérifiées.
- Les accès administrateurs ne sont pas suffisamment sécurisés.
- Le réseau interne manque de segmentation.
- La supervision des équipements est insuffisante.
- Aucun processus formalisé de gestion des incidents de sécurité n'existe.

La direction a validé un projet de modernisation d'une durée de **12 semaines**.

Vous êtes chargés de mettre en place un environnement de pilotage permettant aux équipes techniques et à la direction de suivre l'avancement des travaux.

Vous utiliserez GitHub Issues et GitHub Projects pour organiser, planifier et visualiser ce projet.

---

## Partie 1 — Initialisation du projet

Créer un dépôt GitHub intitulé `infra-modernisation`.

Ce dépôt servira à centraliser les travaux techniques, les demandes d'intervention et la documentation du projet.

Créer ensuite un GitHub Project associé au dépôt, intitulé **Modernisation Infrastructure & Sécurité**.

Le projet doit permettre de suivre les travaux depuis leur planification jusqu'à leur validation.

À ce stade, vous devez disposer d'un dépôt et d'un espace de gestion de projet opérationnels.

## Partie 2 — Définition des tâches et des jalons

### 2.1 — Création des issues

Créer au minimum **15 issues**, réparties dans les cinq domaines suivants :

| Domaine | Exemples de travaux |
|---|---|
| Systèmes | Migration de serveurs, mises à jour, durcissement Linux |
| Réseaux | VLAN, pare-feu, VPN, segmentation |
| Cybersécurité | MFA, audit de vulnérabilités, gestion des accès |
| Supervision | Centralisation des logs, monitoring, alertes |
| Continuité d'activité | Sauvegardes, restauration, PRA |

Chaque issue doit contenir :

- Un titre explicite.
- Une description du travail attendu.
- Des critères permettant de considérer la tâche comme terminée.

Vous devez définir vous-mêmes les tâches pertinentes, sans vous limiter aux exemples proposés.

### 2.2 — Création des milestones

Le projet doit être structuré autour de quatre jalons :

| Jalon | Échéance |
|---|---|
| Audit et préparation | Fin semaine 2 |
| Modernisation des infrastructures | Fin semaine 6 |
| Sécurisation et supervision | Fin semaine 10 |
| Validation et mise en production | Fin semaine 12 |

Associer les issues aux jalons correspondants.

Vérifier que chaque jalon représente un ensemble cohérent de travaux et qu'il est possible de suivre son avancement.

## Partie 3 — Personnalisation du suivi

Les fonctionnalités standard de GitHub Projects ne suffisent pas à répondre à tous les besoins de l'entreprise.

Vous devez enrichir votre projet à l'aide de **champs personnalisés**.

Créer les champs nécessaires pour gérer les informations suivantes :

| Information | Type attendu |
|---|---|
| Priorité | Choix parmi plusieurs niveaux |
| Domaine technique | Choix parmi les cinq domaines |
| Charge estimée | Nombre de jours |
| Risque | Niveau de risque |
| Date de début | Date |
| Date de fin prévue | Date |
| Avancement | Statut du travail |

Les valeurs exactes des champs et leur configuration sont à votre initiative.

Renseigner ces informations sur l'ensemble des tâches, en veillant à conserver une cohérence entre priorité, risque, charge et planification.

## Partie 4 — Création de vues adaptées aux utilisateurs

La direction, le responsable technique et les intervenants n'ont pas besoin de consulter les mêmes informations.

Votre objectif est de créer plusieurs vues du même projet, adaptées à leurs usages.

### Vue 1 — Tableau opérationnel

Créer une vue Kanban regroupant les tâches selon leur état d'avancement.

Les cartes doivent afficher les informations utiles au suivi quotidien.

Prévoir au moins une tâche bloquée et plusieurs tâches en cours.

### Vue 2 — Suivi des charges

Créer une vue sous forme de tableau :

- Regroupée par domaine technique.
- Affichant les charges estimées.
- Permettant de connaître la charge totale de chaque domaine.
- Permettant de connaître la charge globale du projet.

Utiliser les fonctionnalités d'agrégation de GitHub Projects.

### Vue 3 — Roadmap

Créer une vue chronologique représentant la planification des travaux sur les 12 semaines.

Les dates doivent être cohérentes avec les milestones.

Identifier les tâches pouvant être réalisées en parallèle et celles présentant des dépendances.

### Vue 4 — Synthèse de direction

Configurer une vue synthétique permettant de visualiser rapidement :

- Les travaux prioritaires.
- Les tâches présentant un risque élevé.
- Les interventions restant à terminer.

Cette vue doit permettre à la direction d'identifier rapidement les points nécessitant son attention.

## Partie 5 — Tableaux de bord et graphiques

La direction souhaite disposer d'indicateurs visuels pour suivre l'évolution du projet sans consulter chaque issue.

À l'aide des fonctionnalités d'analyse de GitHub Projects (Insights), créer au minimum **trois graphiques** :

1. Un graphique présentant la répartition des tâches par domaine technique.
2. Un graphique montrant la répartition des tâches selon leur état d'avancement.
3. Un graphique permettant d'identifier les tâches selon leur priorité ou leur niveau de risque.

Choisir les types de graphiques les plus pertinents et configurer les regroupements nécessaires.

Les graphiques doivent exploiter les informations du projet et non des données saisies indépendamment.

## Partie 6 — Traçabilité des interventions avec Git

Dans le cadre du projet de modernisation, certaines interventions nécessitent la création ou la modification de scripts et de fichiers de configuration.

L'entreprise souhaite pouvoir retrouver facilement les modifications réalisées pour chaque intervention et identifier les commits associés aux tâches.

### 6.1 — Réalisation d'interventions techniques

Choisir **deux issues existantes** parmi les travaux prévus dans le projet.

Pour chacune d'elles, réaliser une modification technique dans le dépôt GitHub.

Les interventions peuvent notamment porter sur :

| Domaine | Exemple de réalisation |
|---|---|
| Systèmes | Script Bash de vérification de l'espace disque |
| Réseaux | Fichier de configuration d'un pare-feu |
| Cybersécurité | Script de contrôle des permissions sensibles |
| Supervision | Script de vérification de disponibilité de serveurs |
| Sauvegardes | Script Bash d'archivage et de sauvegarde |

Les réalisations doivent être simples, mais fonctionnelles et cohérentes avec les issues sélectionnées.

### 6.2 — Association des commits aux issues

Pour chaque intervention :

1. Réaliser le travail dans une branche dédiée.
2. Effectuer au moins deux commits représentant des étapes distinctes du travail.
3. Associer explicitement les commits à l'issue concernée.
4. Publier les modifications sur GitHub.
5. Créer une Pull Request permettant d'intégrer les modifications dans la branche principale.
6. Faire en sorte que la Pull Request soit également associée à l'issue correspondante.

L'historique Git doit permettre de comprendre les modifications réalisées et de retrouver facilement les travaux associés à chaque issue.

**Attention :** la simple mention d'un numéro d'issue dans un commit ne provoque pas nécessairement sa fermeture. Il faut distinguer la référence à une issue et les mots-clés permettant sa fermeture automatique lors de l'intégration d'une Pull Request.

### 6.3 — Validation et suivi

Une fois les modifications intégrées :

- Vérifier que les commits sont consultables depuis les issues concernées.
- Vérifier la présence des Pull Requests associées.
- Actualiser les statuts dans GitHub Projects.
- Vérifier que les changements sont correctement représentés dans les vues et les indicateurs du projet.

### 6.4 — Correction d'une intervention

Pour l'une des deux interventions, simuler une correction après une première version.

Cette correction doit faire l'objet d'un nouveau commit, dont le message permet de comprendre le problème corrigé.

L'objectif est de conserver une traçabilité complète de l'intervention initiale et de sa correction.

## Partie 7 — Simulation de l'avancement du projet

Le projet est désormais configuré. Vous devez simuler son évolution.

Nous sommes à la fin de la quatrième semaine.

La direction vous transmet les informations suivantes :

- L'audit initial est terminé.
- Deux opérations de migration de serveurs ont été réalisées.
- Une intervention réseau est bloquée à cause d'un équipement non livré.
- Une vulnérabilité critique a été découverte sur un serveur exposé.
- La configuration de la supervision a commencé.
- Le déploiement du MFA a pris du retard.

Mettre à jour les issues, les statuts, les priorités et la planification pour représenter cette situation.

Créer une nouvelle issue concernant la vulnérabilité critique, avec un niveau de priorité adapté.

Actualiser la roadmap et vérifier les conséquences sur les vues et graphiques.

## Partie 8 — Analyse et restitution

Rédiger dans le `README.md` du dépôt une courte synthèse destinée à la direction, répondant aux questions suivantes :

1. Quel est le volume total de travail estimé pour le projet ?
2. Quel domaine technique représente la charge la plus importante ?
3. Quels travaux présentent les risques les plus élevés ?
4. Quelles tâches risquent de retarder le projet ?
5. Quels changements de priorité recommandez-vous après la découverte de la vulnérabilité critique ?

La synthèse doit s'appuyer sur les informations visibles dans GitHub Projects.

---

## Livrables attendus

À la fin du TP, fournir :

- L'URL du dépôt GitHub contenant les issues, les scripts, les configurations et le README.
- L'URL du GitHub Project.
- Un projet comportant les champs personnalisés, les milestones, les vues et les graphiques demandés.
- Une roadmap cohérente avec les échéances du projet.
- Au moins deux interventions techniques versionnées et associées à leurs issues.
- Les Pull Requests correspondant aux interventions.
- Une synthèse de l'état du projet à la fin de la quatrième semaine.

Le dépôt et le projet doivent être accessibles à l'enseignant.

## Critères d'évaluation

| Critère | Points |
|---|---:|
| Issues et milestones | 4 |
| Champs personnalisés | 3 |
| Vues et agrégations | 3 |
| Roadmap | 2 |
| Graphiques | 2 |
| Commits, branches et Pull Requests associés aux issues | 4 |
| Simulation et analyse | 2 |
| **Total** | **20** |

## Bonus — Automatisation du suivi

Pour aller plus loin, mettre en place au moins une automatisation avec les workflows intégrés de GitHub Projects.

Cette automatisation doit permettre de faire évoluer le suivi du projet en fonction d'un événement survenant sur une issue ou une Pull Request.

Expliquer brièvement son fonctionnement dans le README.
