# 🌍 Analyse de la situation sanitaire en Afrique de l'Ouest

> Tableau de bord analytique interactif sur le paludisme et la mortalité maternelle au Sénégal et dans quatre pays voisins.

![Python](https://img.shields.io/badge/Python-3.13.7-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.x-green)
![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow)
![Licence](https://img.shields.io/badge/Données-CC%20BY%204.0-orange)

---

## 📋 Description du projet

Ce projet s'inscrit dans le cadre du **Certificat Data Analysis**. Il vise à concevoir un pipeline complet d'analyse de données de santé publique — depuis la collecte des données brutes jusqu'à la production d'un tableau de bord interactif sous Power BI Desktop.

Les indicateurs analysés sont :
- 🦟 **Incidence du paludisme** (pour 1 000 personnes à risque)
- 👩 **Taux de mortalité maternelle** (pour 100 000 naissances vivantes)
- 🏥 **Couverture en soins prénataux** (% de femmes ayant eu au moins une visite)

**Pays couverts :** Sénégal, Guinée, Mali, Burkina Faso, Côte d'Ivoire

**Période :** 2000 – 2024 (selon l'indicateur)

---

## 🗂️ Structure du projet

```
projet-sante-afrique-ouest/
│
├── data/                          # Données brutes téléchargées
│   ├── paludisme.csv
│   ├── mortalite_maternelle.csv
│   └── soins_prenataux.csv
│
├── notebooks/                     # Notebooks Jupyter
│   └── 01_exploration.ipynb       # EDA, nettoyage, export
│
├── exports/                       # Données nettoyées et graphiques
│   ├── paludisme_propre.xlsx
│   ├── mortalite_maternelle_propre.xlsx
│   ├── soins_prenataux_propre.xlsx
│   ├── graphique_paludisme_evolution.png
│   ├── graphique_paludisme_barres.png
│   ├── graphique_mortalite_evolution.png
│   ├── graphique_mortalite_barres.png
│   ├── graphique_prenatal_evolution.png
│   └── graphique_prenatal_barres.png
│
├── README.md                      # Ce fichier
└── requirements.txt               # Dépendances Python
```

---

## 🔧 Installation et lancement

### Prérequis
- Python 3.10 ou supérieur
- Jupyter Notebook
- Power BI Desktop (gratuit, Windows uniquement)

### 1. Cloner le dépôt

```bash
git clone https://github.com/TON_USERNAME/projet-sante-afrique-ouest.git
cd projet-sante-afrique-ouest
```

### 2. Installer les dépendances

```bash
pip install -r requirements.txt
```

### 3. Lancer le notebook

```bash
jupyter notebook notebooks/01_exploration.ipynb
```

### 4. Ouvrir le tableau de bord Power BI

Ouvrir le fichier `.pbix` dans Power BI Desktop.
Les données sont chargées depuis le dossier `exports/`.

---

## 📊 Résultats et insights clés

### 🦟 Paludisme
- **Burkina Faso** est le pays le plus touché avec une moyenne de **475 cas/1 000** personnes à risque
- **Le Sénégal** se distingue nettement avec seulement **80 cas/1 000** — 4 à 6 fois moins que les autres pays
- Tendance globale à la **baisse sur 2000-2024**, reflétant les efforts de lutte antipaludique

### 👩 Mortalité maternelle
- **La Guinée** présente la situation la plus critique avec **888 décès/100 000** naissances en moyenne
- **Le Mali** partait d'un niveau catastrophique en 1985 (1 341 décès) mais montre une amélioration progressive
- **Le Sénégal** affiche le meilleur résultat avec **257 décès/100 000** en 2019

### 🏥 Soins prénataux
- Progression spectaculaire au **Sénégal** : de 29.7% en 1986 à **97.7% en 2019**
- Tous les pays montrent une **tendance à la hausse** sur la période
- Données basées sur des **enquêtes ponctuelles** (EDS) — pas de données après 2019

---

## ⚠️ Limites et biais

- Les données de soins prénataux sont **irrégulières** (enquêtes tous les 2-5 ans)
- Possible **sous-déclaration** dans les zones rurales et reculées
- Les données de mortalité maternelle s'arrêtent en **2020** — impact COVID-19 non mesuré
- Les données de soins prénataux s'arrêtent en **2019**

---

## 📦 Dépendances

```
pandas
numpy
matplotlib
seaborn
jupyter
openpyxl
requests
```

---

## 🗃️ Sources des données

| Indicateur | Source | Licence |
|---|---|---|
| Incidence du paludisme | Our World in Data / OMS | CC BY 4.0 |
| Mortalité maternelle | Our World in Data / OMS | CC BY 4.0 |
| Soins prénataux | Our World in Data / OMS | CC BY 4.0 |

> Les données sont publiées par Our World in Data sous licence [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). La source originale est l'Organisation Mondiale de la Santé (OMS / Global Health Observatory).

---

## 👤 Auteur

Projet réalisé dans le cadre du **Certificat Data Analysis**

---

## 📄 Licence

Ce projet est open source. Les données utilisées sont sous licence CC BY 4.0 — citation de la source obligatoire.
