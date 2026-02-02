# 📊 Application Django – Import et Analyse de Données Excel
# 📊 Django Application – Excel Data Import and Analysis

## FR (Français)

### 📌 Description
Cette application Django permet d’importer des fichiers Excel contenant des données de consommation, de filtrer ces données sur une période donnée, puis d’effectuer des calculs statistiques et analytiques avancés. Elle est conçue pour gérer des volumes de données importants grâce à Pandas et Dask. Les résultats sont stockés en base de données et affichés via des pages web dynamiques.

## EN (English)

### 📌 Description
This Django application allows importing Excel files containing consumption data, filtering these data over a selected period, and performing advanced statistical and analytical calculations. It is designed to handle large volumes of data using Pandas and Dask. The results are stored in a database and displayed through dynamic web pages.

## 🚀 Fonctionnalités | Features

FR :
- Importation de fichiers Excel
- Sélection dynamique des colonnes
- Filtrage par période (date de début / date de fin)
- Traitement des données avec Pandas et Dask
- Calculs statistiques : minimum, maximum, moyenne
- Calcul du pas de consommation
- Consommation par heure, jour, semaine, mois et année
- Génération de vecteurs de consommation
- Compression et stockage des données (JSON, gzip, base64)
- Sauvegarde des résultats en base de données
- Visualisation des données traitées

EN :
- Excel file import
- Dynamic column selection
- Period filtering (start date / end date)
- Data processing with Pandas and Dask
- Statistical calculations: minimum, maximum, average
- Consumption step calculation
- Consumption per hour, day, week, month, and year
- Generation of consumption vectors
- Data compression and storage (JSON, gzip, base64)
- Saving results to the database
- Visualization of processed data

## 🛠️ Technologies utilisées | Technologies Used
- Python 3
- Django
- Pandas
- Dask
- OpenPyXL
- HTML / Django Templates
- SQLite (default)

## 📁 Structure du projet | Project Structure
project/
├── app/
│   ├── views.py
│   ├── models.py
│   ├── forms.py
│   └── templates/
├── media/
│   └── file/
├── manage.py
└── requirements.txt

## 📥 Utilisation | Usage

FR :
1. Importer un fichier Excel
2. Choisir la colonne de consommation
3. Définir la période (date de début et date de fin)
4. Définir la valeur maximale, le nombre de classes et le coefficient
5. Lancer le traitement
6. Consulter les résultats calculés et sauvegardés

EN :
1. Import an Excel file
2. Select the consumption column
3. Define the period (start date and end date)
4. Set the maximum value, number of classes, and coefficient
5. Run the processing
6. View the calculated and saved results

## ▶️ Installation et exécution | Installation & Run

git clone <repository-url>
cd project
python -m venv venv
source venv/bin/activate   # Linux / Mac
venv\Scripts\activate      # Windows
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

Application URL :
http://127.0.0.1:8000/

## ⚠️ Prérequis | Requirements

FR :
- Python 3.9 ou plus
- Pip
- Virtualenv recommandé
- Ressources suffisantes pour le traitement avec Dask

EN :
- Python 3.9 or higher
- Pip
- Virtualenv recommended
- Sufficient resources for Dask processing



