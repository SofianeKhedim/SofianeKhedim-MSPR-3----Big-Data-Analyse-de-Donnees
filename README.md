# MSPR Big Data & Analyse de Données

## Description du Projet

Ce projet consiste en une preuve de concept (POC) pour prédire les tendances électorales en utilisant l'intelligence artificielle. Réalisé dans le cadre de la certification RNCP Expert en Informatique et Système d'Information, il vise à démontrer la faisabilité d'un modèle prédictif basé sur des indicateurs socio-économiques.

### Objectif
Développer un outil capable de prédire les résultats électoraux dans un secteur géographique restreint en analysant différents facteurs comme la démographie, l'économie, la sécurité et la société.

## Contexte Client

**Client fictif** : Jean-Edouard de la Motte Rouge
- Start-up spécialisée dans le conseil en campagnes électorales
- **Besoin** : Obtenir un avantage concurrentiel grâce à l'IA prédictive

## Zone d'Étude : Normandie

**Justification du choix :**
- Population : ~3,3 millions d'habitants
- 5 départements : Calvados, Eure, Manche, Orne, Seine-Maritime
- Diversité urbain/rural représentative
- Résultats 2022 : Macron 55,84% vs Le Pen 44,16%

## Données et Indicateurs Analysés

### Sources de données
- **Élections** : Résultats présidentielles 2017 & 2022
- **Démographie** : INSEE (population, classes sociales, âge)
- **Sécurité** : Data.gouv.fr (taux de criminalité)
- **Économie** : Création d'entreprises

### Critères sélectionnés
- **Taux de criminalité** - Impact sur le sentiment d'insécurité
- **Création d'entreprises** - Dynamisme économique local
- **Structure sociale** - Classes populaires vs classes supérieures
- **Taux d'abstention** - Défiance institutionnelle
- **Part des étrangers** - Influence sur les débats migratoires
- **Indice de jeunesse** - Priorités générationnelles
- **Taille de population** - Contexte urbain/rural

## Méthodologie

### Gestion de projet
- **Méthode** : Agile (Scrum adapté)
- **Outil de suivi** : Jira
- **Équipe** : 5 membres avec répartition des tâches

### Architecture technique
```
Données brutes → Nettoyage → Fusion → Dataset final → Modélisation
     ↓              ↓          ↓          ↓           ↓
  [2017/2022]   [ETL]    [Join communes] [ML Ready] [Prédictions]
```

### Technologies utilisées
- **Langage** : Python
- **Environnement** : Google Colab, Jupyter Notebook
- **Bibliothèques** : 
  - Pandas, NumPy (manipulation de données)
  - Scikit-learn (machine learning)
  - Matplotlib (visualisation)

## Modèles Testés

| Modèle | Type | Performance |
|--------|------|-------------|
| **XGBoost** | Gradient Boosting | Meilleur |
| Random Forest | Ensemble | Bon |
| Gradient Boosting | Boosting | Bon |
| Régression Logistique | Linéaire | Correct |
| K-Nearest Neighbors | Instance-based | Moyen |

### Métriques d'évaluation
- **Accuracy** : Précision globale
- **Precision** : Exactitude par classe
- **Recall** : Couverture par classe  
- **F1-Score** : Équilibre précision/rappel

## Structure du Projet

```
📦 MSPR-BigData-Elections/
├── 📁 database/
│   ├── dataset_global.db
│   ├── dataset_normandie.db
├── Rapport MSPR 3 - Big Data & Analyse de Données.pdf
├── dataset_final_global.csv
├── dataset_normandie.csv
├── dataset_normandie.sql
├── dataset_sqlite_global.sql
```

## 👥 Équipe

- **BADREDDINE KHALIL**
- **KHEDIM SOFIANE** 
- **REGUIEG ZAKARIA**
- **GHANMI AHMED**
- **ISMAIL ALI**

**Encadrant** : BOUFADEN HEDI

## 🏫 Institution

**EPSI Paris** - Année Universitaire 2024-2025  
Certification RNCP N°35584 - Expert en Informatique et Système d'Information

## 📚 Sources

- [Résultats électoraux - Ministère de l'Intérieur](https://www.resultats-elections.interieur.gouv.fr)
- [INSEE - Données démographiques](https://www.insee.fr)
- [Data.gouv.fr - Données publiques](https://www.data.gouv.fr)
- [Données électorales](https://www.data.gouv.fr/fr/pages/donnees-des-elections/)
- [Données sécurité](https://www.data.gouv.fr/fr/pages/donnees-securite/)

## ⚖️ Conformité

Ce projet respecte les exigences du **RGPD**.
---
