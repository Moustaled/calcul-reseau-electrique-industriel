# Projet d'Installations Électriques Industrielles — Usine d'Injection Plastique

<p align="center">
  <img src="https://img.shields.io/badge/Catégorie-Projet%20Académique-blue" alt="Catégorie : Projet Académique">
  <img src="https://img.shields.io/badge/Logiciel-AutoCAD-C81F2E?logo=autodesk" alt="Logiciel : AutoCAD">
  <img src="https://img.shields.io/badge/Logiciel-DIALux-005A9B" alt="Logiciel : DIALux">
</p>

> [Projet Académique] Projet complet d'installations électriques et de licenciement (DGEG) pour une usine d'injection plastique, comprenant le calcul des puissances (~700 kVA), l'étude d'éclairage (DIALux), les schémas AutoCAD et le dimensionnement des protections (régime TT).

---

## Sommaire

- L'Énoncé et l'Objectif Technique
- Architecture du Système : Alimentation, Distribution et Protections
- Méthodologie de Projet et Outils Utilisés
- Solutions Techniques Mises en Œuvre
- Intégration et Flux de Travail
- Résultats Techniques, Conformité et Difficultés
- Conclusion et Apprentissages Techniques
- Documentation du Projet (Pièces Écrites et Dessinées)
- Licence

---

### 1. L'Énoncé et l'Objectif Technique

Ce projet intégré a été développé dans le cadre de l'unité d'enseignement **Projet d'Installations Électriques (PIIE)**, inscrite au plan d'études du CTeSP d'Installations Électriques de l'ESTGA – Université d'Aveiro, pour l'année universitaire 2022/2023.

L'objectif central était d'élaborer le **projet électrique complet d'une unité industrielle**, depuis l'évaluation de la puissance électrique prévisible jusqu'à la préparation des pièces écrites et dessinées nécessaires au licenciement auprès de la **DGEG (Direction Générale de l'Énergie et de la Géologie)**.

Les spécifications techniques obligatoires comprenaient :
- L'évaluation de la puissance électrique prévisible à partir des machines de l'usine.
- L'étude d'éclairage de tous les espaces, à l'aide d'un logiciel spécialisé.
- L'élaboration des **Pièces Écrites** : mémoire descriptive et justificative, fiches de caractérisation (MT/HT, Réseau BT, Installation BT) et notes de calcul justificatives.
- L'élaboration des **Pièces Dessinées** : plans de localisation, tracé des chemins de câbles, emplacement des tableaux, schéma du réseau et schémas électriques de principe (ELP).
- Le remplissage de la documentation de licenciement : Fiche Électrotechnique, Terme de Responsabilité et Identification du Projet.

### 2. Architecture du Système : Alimentation, Distribution et Protections

La structure du projet est définie par le système d'alimentation et de distribution, conçu pour garantir la continuité, la sécurité et l'efficacité.

- **Poste de Transformation (PT) :** L'usine est alimentée par une ligne souterraine de 15 kV (neutre mis solidement à la terre, puissance de court-circuit de 350 MVA). Le PT est une cabine basse préfabriquée, équipée de cellules MT, d'un transformateur et du Tableau Principal de Transformation (QPT).

- **Tableau Général Basse Tension (QGBT) :** À partir du QPT, l'énergie est distribuée par le QGBT, qui alimente :
  - 7 tableaux partiels (QP1 à QP7) pour la force motrice et les prises ;
  - 1 tableau indépendant pour l'éclairage (QPI) ;
  - 1 Tableau Général de Mobilité (QGM) pour les bornes de recharge de véhicules électriques.

- **Calcul des Puissances et Équilibrage :** À partir de 25 équipements principaux (presses à injecter, broyeur de 70 kVA, etc.), la puissance prévisible totale atteint environ **700 kVA**. L'équilibrage entre phases a été optimisé afin d'éviter des déséquilibres supérieurs à 15 %.

- **Système de Protections :** Le régime **TT** a été retenu, avec le neutre relié à la terre de service et les masses reliées à la terre de protection. La protection contre les contacts indirects est assurée par des disjoncteurs différentiels. La résistance du réseau de terre a été dimensionnée pour un maximum de 20 Ω.

- **Chemins de Câbles et Conduits :** Les câbles ont été dimensionnés en fonction du courant de service et de la chute de tension admissible. Le diamètre des conduits suit la règle : `∅conduit = 0,33 × Σ section des câbles`.

### 3. Méthodologie de Projet et Outils Utilisés

| Outil | Finalité |
| :--- | :--- |
| **AutoCAD** | Production de toutes les pièces dessinées (plans, schémas, synoptiques). |
| **DIALux** | Étude d'éclairage, simulation des niveaux d'éclairement et sélection des luminaires. |
| **Excel** | Notes de calcul justificatives (équilibrage, dimensionnement des câbles, chutes de tension). |
| **Word** | Rédaction de la mémoire descriptive et des fiches de caractérisation DGEG. |

L'ensemble des pièces dessinées comprend les plans de localisation, le tracé des chemins de câbles, l'emplacement des tableaux, l'alimentation des équipements, l'éclairage normal/de secours, le schéma unifilaire et les schémas électriques de principe (ELP) de tous les tableaux.

### 4. Solutions Techniques Mises en Œuvre

- **Alimentation des Machines :** Circuits dédiés avec protections thermomagnétiques et différentielles adaptées aux courants de démarrage et au régime nominal.
- **Circuits de Prises :** Circuits d'usage général (maximum 8 points par circuit) et circuits spécifiques pour les équipements critiques.
- **Bornes de Recharge pour Véhicules Électriques :** Le QGM alimente des bornes de recharge avec protections différentielles de type A et circuits indépendants, conformément à la réglementation en vigueur.
- **Réseau de Terre :** Dimensionné avec des conducteurs en cuivre nu de 50 mm² et des électrodes en acier cuivré, afin de garantir une résistance de terre < 20 Ω.

### 5. Intégration et Flux de Travail

Le projet a suivi un flux logique et planifié :
1.  Relevé des exigences et analyse de l'énoncé.
2.  Calculs préliminaires des puissances et de l'équilibrage.
3.  Étude d'éclairage avec DIALux.
4.  Élaboration du schéma unifilaire et de l'architecture des tableaux.
5.  Dessin technique sous AutoCAD de tous les plans et schémas.
6.  Dimensionnement détaillé des câbles, des protections et des conduits.
7.  Rédaction de la mémoire descriptive et remplissage des annexes officielles de la DGEG.
8.  Consolidation de l'ensemble du dossier dans un portfolio numérique.

### 6. Résultats Techniques, Conformité et Difficultés Surmontées

- **Résultat Final :** Le projet a pleinement satisfait aux exigences normatives et aux objectifs de l'énoncé, avec une puissance totale prévisible d'environ 700 kVA, un système de protections TT complet, un éclairage validé sous DIALux et une documentation mise en forme pour le licenciement.
- **Difficultés Surmontées :**
  - **Synthèse de la Mémoire Descriptive :** La limite de 5 pages a exigé une synthèse rigoureuse sans perte de contenu technique.
  - **Application Pratique de la Théorie :** Traduction des normes (R.T.I.E.B.T.) et des concepts théoriques en un projet réel et complexe.
- **Piste d'Amélioration Proposée :** Ajout de vues frontales en 2D des tableaux électriques dans les pièces dessinées, pour une meilleure lisibilité.

### 7. Conclusion et Apprentissages Techniques

Ce projet a servi d'intégrateur pratique des connaissances en électrotechnique, en normalisation, en dessin technique et en gestion de projet. Le principal apprentissage a été de comprendre les phases de création d'un projet d'installations électriques et de développer la capacité à raisonner du point de vue du concepteur.

**Apprentissages techniques spécifiques :**
- Application concrète du R.T.I.E.B.T., des normes européennes et des procédures de la DGEG.
- Importance de l'équilibrage des phases et du choix des protections en milieu industriel.
- Maîtrise d'outils professionnels tels qu'AutoCAD et DIALux.
- Structuration d'une documentation technique complexe en vue du licenciement.

**Perspectives d'Amélioration Technique Future :**
- Mise en place d'un système de suivi des consommations (SCADA / Gestion de l'Énergie).
- Intégration d'une production photovoltaïque en autoconsommation.
- Approfondissement de l'étude des harmoniques générées par les machines.
- Utilisation de tableaux modulaires intelligents avec communication pour la maintenance prédictive.

### 8. Documentation du Projet (Pièces Écrites et Dessinées)

Toute la documentation technique, comprenant la mémoire descriptive, les annexes DGEG remplies, la feuille de calcul d'équilibrage et les fichiers DWG, est disponible pour consultation et téléchargement dans le dossier `project-files/` de ce dépôt.

*Remarque : la mémoire descriptive fournie est un exemple représentatif, destiné à protéger les données sensibles du document original remis pour évaluation.*

### 9. Licence

Ce projet est distribué sous **licence MIT**. Voir le fichier `LICENSE` pour plus de détails.
