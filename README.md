# Analyse E-Commerce Maroc - Pipeline Complet de Nettoyage et d'Analyse

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Excel](https://img.shields.io/badge/Excel-Data%20Source-green)

## Aperçu du Projet

Ce projet présente un pipeline complet d'analyse de données e-commerce pour des données de vente marocaines. Il suit une méthodologie rigoureuse allant de l'inspection initiale jusqu'au reporting final, en passant par le nettoyage des données et l'analyse exploratoire.

**Objectifs Principaux:**
- Nettoyer et préparer un jeu de données e-commerce réaliste avec anomalies
- Identifier et corriger les problèmes de qualité des données
- Extraire des insights métier actionnables
- Créer un workflow reproductible pour l'analyse de données

## 🛠️ Stack Technologique

| Technologie | Version | Utilisation |
|-------------|---------|-------------|
| **Python** | 3.8+ | Langage de programmation principal |
| **Pandas** | 1.3+ | Manipulation et analyse des données |
| **NumPy** | 1.21+ | Calculs numériques |
| **Matplotlib** | 3.4+ | Visualisations de base |
| **Seaborn** | 0.11+ | Visualisations statistiques |
| **Jupyter** | 6.4+ | Environnement de développement |
| **OpenPyXL** | 3.0+ | Lecture des fichiers Excel |

## 📊 Structure du Pipeline

### 1. **Inspection Initiale des Données**
- Chargement du dataset `morocco_ecommerce_anomalies.xlsx`
- Analyse de la structure (shape, types de données)
- Identification des problèmes structurels

### 2. **Analyse des Valeurs Manquantes**
- Détection des valeurs manquantes par colonne
- Classification en champs critiques/semi-critiques/optionnels
- Stratégie de traitement adaptée

### 3. **Nettoyage des Types de Données**
- Conversion des colonnes numériques corrompues
- Gestion des entrées texte dans les champs numériques
- Validation des conversions

### 4. **Standardisation des Données Catégorielles**
- Nettoyage des noms de villes et régions
- Unification des variantes (ex: "Casa" → "Casablanca")
- Normalisation de la casse et des espaces

### 5. **Validation des Dates**
- Conversion en format datetime
- Détection des dates invalides
- Extraction de features temporelles

### 6. **Détection des Doublons**
- Identification des doublons complets
- Gestion des order_id dupliqués
- Stratégie de conservation/déduplication

### 7. **Traitement des Valeurs Aberrantes**
- Méthodes IQR et Z-score
- Analyse des commandes extrêmes
- Stratégie de traitement raisonnée

### 8. **Analyse Exploratoire (EDA)**
- Statistiques descriptives
- Analyse par région et catégorie
- KPIs de performance

### 9. **Analyse Temporelle**
- Tendances mensuelles
- Saisonnalité et pics
- Performance dans le temps

### 10. **Reporting Final**
- Synthèse des insights
- Recommandations métier
- Limitations et prochaines étapes
 
## Installation et Exécution

### Prérequis
```bash
python -m venv ecommerce_env
source ecommerce_env/bin/activate  # Linux/Mac
# ou
ecommerce_env\Scripts\activate    # Windows

pip install -r requirements.txt
```

### Fichier requirements.txt
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
openpyxl>=3.0.0
```
## 📞 Contact et Support

Pour toute question concernant ce projet ou la méthodologie utilisée, n'hésitez pas à ouvrir une issue dans le repository du projet.

---
**Note**: Ce projet démontre un workflow complet d'analyse de données adapté aux contextes e-commerce avec des défis de qualité de données réalistes.
 
