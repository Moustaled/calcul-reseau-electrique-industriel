
# Étude et analyse d'un réseau électrique industriel HTA/BT

**Distribution électrique industrielle | Bilan de puissance | Dimensionnement BT | Protections électriques | Schémas unifilaires**

**Projet d'ingénierie — ECAM-EPMI**  
**Spécialité :** ISE (Ingénieur en Système Électrique)

**Équipe :**
- Moustapha IBRAHIM DJAMA
- Thomas DHUNARA
- Mariel FRESNEL

[Portfolio de Moustapha IBRAHIM DJAMA](https://portfolio-eta-ten-t34s52rvq8.vercel.app/)

---

## 1. Présentation du projet

La distribution de l'énergie électrique dans une installation industrielle nécessite une étude rigoureuse des besoins de puissance, du dimensionnement des équipements et de la coordination des dispositifs de protection.

Ce projet porte sur l'analyse d'un **réseau électrique industriel destiné à alimenter une usine d'injection de matières plastiques**.

L'installation étudiée comprend une alimentation moyenne tension de **15 kV**, un poste de transformation HTA/BT et plusieurs tableaux de distribution basse tension assurant l'alimentation des équipements industriels et des circuits auxiliaires.

L'étude vise à comprendre l'architecture électrique de l'installation, à exploiter ses données techniques et à examiner la cohérence des choix de dimensionnement.

Les principaux axes techniques sont :

- Analyse de l'architecture générale HTA/BT.
- Exploitation du bilan de puissance de l'installation.
- Étude des courants d'emploi et des facteurs de simultanéité.
- Analyse du dimensionnement des canalisations électriques.
- Vérification des critères de choix des protections.
- Étude des courants de court-circuit et du pouvoir de coupure.
- Analyse de la distribution des charges entre les tableaux.
- Lecture et exploitation des schémas unifilaires.
- Organisation et synthèse de la documentation technique.

Ce projet mobilise des compétences en électrotechnique, réseaux électriques industriels, distribution basse tension et analyse de documents d'ingénierie.

---

## 2. Présentation de l'installation industrielle

### 2.1 Caractéristiques générales du réseau

L'installation est alimentée par un réseau moyenne tension, puis l'énergie est distribuée vers les différents équipements de l'usine après transformation en basse tension.

| Caractéristique | Donnée de référence |
|---|---|
| Type d'installation | Réseau électrique industriel |
| Activité industrielle | Injection de matières plastiques |
| Tension d'alimentation HTA | 15 kV |
| Distribution basse tension | 400/230 V |
| Fréquence nominale | 50 Hz |
| Régime de liaison à la terre indiqué | TT |
| Tableau principal de distribution | QGBT |
| Tableau de distribution moteurs | QGM |
| Tableaux secondaires | QP1 à QP7 |
| Tableau d'éclairage | QPI |

L'architecture est organisée autour d'un poste de transformation et de plusieurs niveaux de distribution, afin d'assurer l'alimentation des charges industrielles.

### 2.2 Architecture générale du réseau

![Diagramme général du réseau électrique industriel](03_Illustrations/aperçu_plan_03_Diagramme_general_du_reseau.png)

Le diagramme général permet d'identifier les principaux équipements et les liaisons électriques de l'installation.

La structure étudiée comprend notamment :

**Alimentation moyenne tension**

L'énergie électrique est reçue au niveau de l'arrivée 15 kV. Le poste de transformation assure ensuite l'adaptation de la tension aux besoins de la distribution basse tension.

**Tableau de distribution QPT**

Le tableau QPT intervient dans l'organisation de la distribution associée au poste de transformation.

**Tableau général basse tension QGBT**

Le QGBT constitue un élément central de la distribution électrique. Il participe à l'alimentation des différents ensembles fonctionnels de l'installation.

**Tableau QGM**

Le QGM regroupe des départs associés à l'alimentation d'équipements industriels, notamment des moteurs.

**Tableaux secondaires QP1 à QP7**

Les tableaux secondaires permettent de répartir l'alimentation électrique entre différents secteurs et équipements.

**Tableau QPI**

Le tableau QPI est associé à la distribution des circuits d'éclairage.

Cette organisation permet une distribution structurée et facilite l'identification des équipements et des dispositifs de protection.

---

## 3. Étude du poste de transformation HTA/BT

Le poste de transformation constitue l'interface entre le réseau moyenne tension et la distribution électrique basse tension de l'usine.

Son analyse repose notamment sur :

- Les caractéristiques du réseau d'alimentation.
- Les besoins électriques de l'installation.
- Le bilan de puissance apparent.
- Le choix de la puissance du transformateur.
- Les caractéristiques des protections.
- Les conditions de raccordement.
- Les contraintes d'exploitation et de sécurité.

### Schéma du poste de transformation

![Schéma unifilaire du poste de transformation QPT](03_Illustrations/aperçu_plan_05_Schema_unifilaire_du_QPT.png)

### Principe de dimensionnement

La puissance nominale du transformateur doit être adaptée à la puissance apparente maximale appelée par l'installation.

Une première condition de dimensionnement s'écrit :

$$
S_n \geq S_{\mathrm{appel,max}}
$$

Avec :

- **Sn** : puissance nominale du transformateur (kVA).
- **Sappel,max** : puissance apparente maximale appelée (kVA).

La détermination de cette puissance nécessite l'analyse des charges, de leurs conditions de fonctionnement et des facteurs de simultanéité.

Le choix final tient également compte des conditions de surcharge, des perspectives d'évolution et des caractéristiques du réseau.

---

## 4. Bilan de puissance de l'installation

Le bilan de puissance constitue une étape essentielle pour déterminer les besoins électriques du site industriel.

Il permet de regrouper les différentes charges, d'estimer leur contribution à la consommation globale et de disposer des grandeurs nécessaires au dimensionnement de l'installation.

### 4.1 Données extraites du dossier technique

| Élément | Puissance apparente indiquée |
|---|---:|
| Liaison QPT–QGBT | 717,871 kVA |
| QGBT | 589,213 kVA |
| QGM | 208,421 kVA |
| Départ QP4 | 78,858 kVA |

Ces valeurs proviennent de documents techniques de référence. Elles constituent les données de départ de l'analyse et doivent être rapprochées des hypothèses de calcul utilisées dans les différentes fiches.

Les écarts entre puissances peuvent notamment dépendre du périmètre de calcul, des facteurs de simultanéité et des conditions de fonctionnement retenues.

### 4.2 Calcul de la puissance apparente

Pour un récepteur triphasé équilibré :

$$
S = \sqrt{3} \times U \times I
$$

Avec :

- **S** : puissance apparente (VA).
- **U** : tension composée (V).
- **I** : courant de ligne (A).

La puissance active s'exprime par :

$$
P = \sqrt{3} \times U \times I \times \cos\varphi
$$

La puissance réactive est donnée par :

$$
Q = \sqrt{3} \times U \times I \times \sin\varphi
$$

La relation entre les trois puissances est :

$$
S^2 = P^2 + Q^2
$$

Ces équations permettent de relier les puissances électriques aux courants circulant dans les différents départs.

### 4.3 Facteurs d'utilisation et de simultanéité

Dans une installation industrielle, l'ensemble des équipements ne fonctionne pas nécessairement à sa puissance nominale au même instant.

Le bilan peut donc nécessiter l'application de facteurs d'utilisation et de simultanéité.

Une expression simplifiée de la puissance active appelée est :

$$
P_{\mathrm{appel}} = \sum_{i=1}^{n} P_{n,i} \times K_{u,i} \times K_{s,i}
$$

Avec :

- **Pn,i** : puissance nominale du récepteur.
- **Ku,i** : facteur d'utilisation.
- **Ks,i** : facteur de simultanéité retenu pour le périmètre étudié.

Les facteurs doivent être appliqués de façon cohérente avec la méthode de bilan choisie, sans compter plusieurs fois le même effet de simultanéité.

Le fichier Excel du projet sert de support à l'analyse et au rapprochement des données de puissance.

---

## 5. Calcul et vérification des courants électriques

Le calcul des courants constitue une étape déterminante pour le choix des conducteurs et des dispositifs de protection.

Pour un réseau triphasé équilibré :

$$
I_b = \frac{S}{\sqrt{3} \times U}
$$

### Exemple : analyse du départ QP4

Les documents techniques indiquent pour ce départ :

- Puissance apparente : **78,858 kVA**.
- Courant indiqué dans une fiche : **32,59 A**.
- Tension basse tension de référence : **400 V**.

En appliquant la relation triphasée :

$$
I_b = \frac{78\,858}{\sqrt{3} \times 400}
$$

On obtient :

$$
\boxed{I_b \approx 113,8\ \text{A}}
$$

Cette valeur est différente du courant de 32,59 A mentionné dans la documentation.

La comparaison met en évidence un point de cohérence à examiner : les deux valeurs peuvent correspondre à des hypothèses, périmètres ou conditions de calcul différents.

Cet exemple illustre l'importance de confronter les résultats des tableaux de calcul aux équations électriques et aux schémas du réseau.

---

## 6. Dimensionnement des canalisations électriques

Le dimensionnement des câbles doit permettre d'assurer le transport de l'énergie dans des conditions compatibles avec les exigences thermiques, électriques et de sécurité.

Plusieurs paramètres interviennent dans le choix des sections :

- Courant d'emploi du circuit.
- Nature des conducteurs.
- Type d'isolant.
- Mode de pose.
- Température ambiante.
- Regroupement des circuits.
- Longueur de la liaison.
- Chute de tension admissible.
- Contraintes thermiques en court-circuit.

### 6.1 Coordination des courants

La condition usuelle de coordination entre la charge, la protection contre les surcharges et la canalisation est :

$$
I_b \leq I_n \leq I_z
$$

Avec :

- **Ib** : courant d'emploi.
- **In** : courant nominal ou de réglage du dispositif de protection.
- **Iz** : courant admissible corrigé du câble.

D'autres conditions relatives au fonctionnement de la protection contre les surcharges doivent également être vérifiées.

### 6.2 Vérification des chutes de tension

La chute de tension influence les performances des équipements alimentés.

Elle est exprimée en pourcentage :

$$
\Delta U(\%) = \frac{\Delta U}{U_n} \times 100
$$

La vérification tient compte de la longueur de la canalisation, du courant transporté, de la section et des caractéristiques du conducteur.

Une chute de tension excessive peut entraîner :

- Une dégradation des conditions de fonctionnement des moteurs.
- Des difficultés de démarrage.
- Une augmentation des pertes électriques.
- Une alimentation insuffisante de certains récepteurs.

### 6.3 Tenue thermique en court-circuit

La tenue thermique du conducteur peut être examinée, dans les conditions d'application de la méthode adiabatique, à partir de :

$$
I^2t \leq k^2A^2
$$

Avec :

- **I** : courant de court-circuit (A).
- **t** : durée de passage du courant (s).
- **A** : section du conducteur (mm²).
- **k** : coefficient dépendant du conducteur et de son isolation.

Cette vérification complète les critères de courant admissible et de chute de tension.

---

## 7. Étude des dispositifs de protection

La protection de l'installation doit répondre aux risques liés aux surcharges, aux courts-circuits et aux défauts d'isolement.

L'étude des protections s'appuie sur les caractéristiques électriques du réseau et sur l'architecture de distribution.

### 7.1 Protection contre les surcharges

Les dispositifs de protection doivent limiter les échauffements excessifs des canalisations.

Le choix du calibre doit être coordonné avec le courant d'emploi et le courant admissible des conducteurs.

### 7.2 Protection contre les courts-circuits

Le pouvoir de coupure d'un dispositif doit être adapté au courant de court-circuit présumé au point où il est installé.

La vérification repose notamment sur :

- Les caractéristiques du transformateur.
- L'impédance du réseau amont.
- Les caractéristiques des liaisons.
- La position du défaut.
- Les caractéristiques du dispositif de protection.

### 7.3 Sélectivité des protections

La sélectivité vise à limiter les conséquences d'un défaut électrique en favorisant le déclenchement de la protection la plus proche de la zone concernée.

Son analyse peut porter sur :

- Les seuils de déclenchement.
- Les temporisations.
- Les caractéristiques temps-courant.
- La coordination entre protections amont et aval.
- Les tableaux de sélectivité des constructeurs.

### 7.4 Protection des personnes

Le régime de liaison à la terre indiqué dans la documentation est de type **TT**.

Dans ce régime, la protection contre les défauts d'isolement nécessite notamment l'examen des dispositifs différentiels et des conditions de mise à la terre.

La condition de protection peut notamment s'exprimer par :

$$
R_A \times I_{\Delta n} \leq U_L
$$

Avec :

- **RA** : résistance associée à la prise de terre des masses et au conducteur de protection.
- **IΔn** : courant différentiel résiduel assigné.
- **UL** : tension limite conventionnelle de contact.

L'application de cette relation dépend des conditions de l'installation et des prescriptions normatives pertinentes.

---

## 8. Analyse des schémas électriques

La documentation graphique permet de comprendre l'organisation de l'installation et les relations entre les équipements électriques.

### 8.1 Schéma du tableau général basse tension

![Schéma unifilaire du QGBT](03_Illustrations/aperçu_plan_10_Schema_unifilaire_du_QGBT.png)

Le schéma du QGBT permet d'étudier :

- L'organisation de la distribution principale.
- Les départs vers les tableaux secondaires.
- L'implantation des dispositifs de protection.
- Le repérage des circuits.
- Les caractéristiques électriques indiquées sur les plans.

### 8.2 Distribution des circuits d'éclairage

![Plan des circuits d'éclairage du rez-de-chaussée](03_Illustrations/aperçu_plan_20_Circuits_declairage_rez_de_chaussee.png)

L'étude des circuits d'éclairage complète l'analyse de la distribution industrielle.

Elle permet de distinguer les besoins associés aux équipements de production et ceux liés aux installations auxiliaires du bâtiment.

Les plans constituent également un support pour examiner le repérage des circuits et l'organisation des tableaux secondaires.

---

## 9. Analyse technique et cohérence du dossier

L'exploitation des documents techniques repose sur une méthode de lecture et de comparaison des informations.

L'analyse s'articule autour des points suivants :

**Cohérence des puissances**

Comparer les bilans de puissance des différentes fiches avec les valeurs indiquées sur les schémas.

**Cohérence des courants**

Recalculer les courants à partir des puissances et tensions de référence, puis examiner les écarts constatés.

**Dimensionnement des liaisons**

Étudier la correspondance entre les courants, les sections de câbles et les conditions de pose.

**Coordination des protections**

Examiner les caractéristiques des appareils par rapport aux contraintes de l'installation.

**Correspondance entre les documents**

Vérifier que les tableaux, départs et équipements désignés dans les fichiers de calcul correspondent aux éléments des schémas électriques.

Cette démarche permet de développer une lecture critique des documents d'ingénierie et de mieux comprendre les interactions entre les différentes étapes d'une étude de réseau électrique.

---

## 10. Documentation du projet

Le dépôt est organisé de manière à faciliter l'accès aux schémas, aux données de calcul et aux documents d'analyse.

```text
calcul-reseau-electrique-industriel/
│
├── README.md
│
├── 01_Schemas_et_plans_de_reference/
│   └── 28 documents PDF
│
├── 02_Calculs_et_fiches/
│   ├── Tableau_de_puissances_et_equilibrage.xlsx
│   ├── Fiche_01_Caracteristiques_reseau_BT.pdf
│   ├── Fiche_02_Installation_moyenne_tension.pdf
│   └── Fiche_03_Distribution_basse_tension.pdf
│
├── 03_Illustrations/
│   └── 6 aperçus des plans techniques
│
└── 04_Analyse_en_francais/
    ├── Synthese_technique_et_points_a_verifier.pdf
    └── Sources_et_limites.md
```

### Description des dossiers

| Dossier | Contenu |
|---|---|
| `01_Schemas_et_plans_de_reference` | Architecture électrique, schémas unifilaires et plans techniques |
| `02_Calculs_et_fiches` | Bilan de puissance, fichier Excel et fiches de caractéristiques |
| `03_Illustrations` | Aperçus des principaux documents graphiques |
| `04_Analyse_en_francais` | Synthèse technique, observations et traçabilité documentaire |

### Principaux documents

**Tableau de puissances et équilibrage**

Classeur Excel regroupant les données de puissance et les informations nécessaires à l'analyse de la répartition des charges.

**Caractéristiques du réseau basse tension**

Document décrivant les principales données électriques du réseau BT.

**Installation moyenne tension**

Fiche consacrée aux caractéristiques de l'alimentation HTA et aux éléments associés au poste de transformation.

**Distribution basse tension**

Document présentant les caractéristiques des équipements et départs de distribution.

**Synthèse technique**

Document d'analyse en français regroupant les informations essentielles de l'installation et les points de cohérence identifiés.

---

## 11. Outils et environnement technique

| Outil ou domaine | Application dans le dossier |
|---|---|
| Excel | Exploitation du bilan de puissance et des tableaux de calcul |
| AutoCAD | Format et environnement de référence des plans électriques |
| DIALux | Documentation d'éclairage présente dans le dossier technique d'origine |
| Schémas unifilaires | Représentation et compréhension de la distribution électrique |
| Calculs électrotechniques | Puissances, courants, protections et dimensionnement |
| GitHub | Organisation et partage de la documentation technique |

Les logiciels AutoCAD et DIALux sont identifiés dans les documents d'origine ; leur présence dans cette liste ne signifie pas que les trois membres de l'équipe ont eux-mêmes réalisé l'intégralité des plans et simulations correspondants.

---

## 12. Références techniques et normatives

L'analyse s'appuie sur les principes de conception et de protection des installations électriques industrielles.

Les principales références à examiner selon le périmètre sont :

- **IEC 60364** : installations électriques basse tension.
- **NF C 15-100** : installations électriques basse tension en France.
- **NF C 13-100 / NF C 13-200** : installations électriques haute tension, selon leur domaine d'application.
- **Documentation des fabricants** : caractéristiques des transformateurs, câbles, disjoncteurs et dispositifs de protection.
- **Cours d'électrotechnique et de réseaux électriques** : calculs de puissances, courants et court-circuits.

Le choix des textes applicables et de leurs éditions doit être adapté au type d'installation, à la date du projet et aux conditions réglementaires retenues.

---

## 13. Démarche pédagogique et origine des documents

Cette étude s'appuie sur un dossier technique de référence relatif à une installation industrielle d'injection de matières plastiques.

Le travail pédagogique porte sur l'exploitation de cette documentation, sa structuration, la compréhension des choix de distribution et l'analyse de cohérence des grandeurs électriques.

Les schémas et plans de référence proviennent d'un projet technique antérieur. Ils ont été organisés et présentés dans le cadre de l'étude ; ils ne sont pas revendiqués comme des dessins originaux de l'équipe.

Les documents ont fait l'objet d'une adaptation documentaire en français, notamment pour les titres, l'organisation des dossiers et les supports de synthèse.

Les informations sur l'origine des sources, leur réutilisation et les limites de la documentation sont détaillées dans :

[Sources et limites documentaires](04_Analyse_en_francais/Sources_et_limites.md)

Cette approche permet de distinguer les éléments de référence des analyses menées dans le cadre de la formation.

---

## 14. Compétences mobilisées

Le projet permet d'aborder plusieurs compétences essentielles en ingénierie des systèmes électriques :

- Lecture et interprétation de schémas électriques industriels.
- Compréhension d'une architecture de distribution HTA/BT.
- Analyse de bilans de puissance.
- Calcul des grandeurs électriques triphasées.
- Étude des critères de dimensionnement des conducteurs.
- Analyse des protections électriques et de leur coordination.
- Identification des incohérences dans des données techniques.
- Exploitation de fichiers de calcul et de documentation.
- Synthèse et présentation d'informations techniques.

Ces compétences sont directement liées aux activités de bureau d'études électriques, de distribution d'énergie et de conception des installations industrielles.

---

## 15. Équipe du projet

### Moustapha IBRAHIM DJAMA

Élève-ingénieur — ECAM-EPMI  
Spécialité ISE (Ingénieur en Système Électrique)

[Portfolio personnel](https://portfolio-eta-ten-t34s52rvq8.vercel.app/)

### Thomas DHUNARA

Élève-ingénieur — ECAM-EPMI

### Mariel FRESNEL

Élève-ingénieur — ECAM-EPMI

---

**ECAM-EPMI — Projet académique en ingénierie des systèmes électriques**

*Étude d'un réseau électrique industriel : distribution HTA/BT, bilan de puissance, dimensionnement et protection des installations.*
