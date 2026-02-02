# 📊 Application Django – Import et Analyse de Données Excel

## 📌 Description

Cette application Django permet d’importer des fichiers Excel contenant des données de consommation, de filtrer ces données sur une période donnée, puis d’effectuer des calculs statistiques et analytiques avancés.

Elle est conçue pour gérer des volumes de données importants grâce à **Pandas** et **Dask**.  
Les résultats sont stockés en base de données et affichés via des pages web dynamiques.

---

## 🚀 Fonctionnalités

- Importation de fichiers Excel
- Sélection dynamique des colonnes
- Filtrage par période (date de début / date de fin)
- Traitement de données avec Pandas et Dask
- Calculs statistiques :
  - minimum, maximum, moyenne
  - pas de consommation
  - consommation par heure, jour, semaine, mois et année
- Génération de vecteurs de consommation
- Compression et stockage des données (JSON + gzip + base64)
- Sauvegarde des résultats en base de données
- Visualisation des données traitées

---

## 🛠️ Technologies utilisées

- Python 3
- Django
- Pandas
- Dask
- OpenPyXL
- HTML / Django Templates
- SQLite (par défaut)

---

## 📁 Structure du projet

```
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
```

---

## 📥 Utilisation

1. Importer un fichier Excel
2. Choisir la colonne de consommation
3. Définir :
   - la période (date de début et date de fin)
   - la valeur maximale
   - le nombre de classes
   - le coefficient
4. Lancer le traitement
5. Consulter les résultats calculés et sauvegardés

---

## ▶️ Installation et exécution

```bash
git clone <url-du-repo>
cd project
python -m venv venv
source venv/bin/activate   # Windows : venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Accéder ensuite à :
```
http://127.0.0.1:8000/
```

---

## ⚠️ Prérequis

- Python 3.9 ou plus
- Pip
- Virtualenv recommandé
- Ressources suffisantes pour le traitement Dask

---

