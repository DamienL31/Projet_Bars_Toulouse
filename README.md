### Projet_Bars_Toulouse
# Projet Happy Hours à Toulouse

Ce projet a pour objectif de collecter, analyser et présenter les informations sur les happy hours des bars à Toulouse en utilisant des techniques de web scraping, d'analyse de données, de visualisation et d'envoi d'e-mails.

## Table des Matières

- [Description du Projet](#description-du-projet)
- [Technologies Utilisées](#technologies-utilisées)
- [Étapes du Projet](#étapes-du-projet)
  - [Partie 1 : Extraction des Données](#partie-1--extraction-des-données)
  - [Partie 2 : Analyse des Données](#partie-2--analyse-des-données)
  - [Partie 3 : Rapport par E-mail](#partie-3--rapport-par-e-mail)
  - [Partie 4 : Cartographie (Bonus)](#partie-4--cartographie-bonus)
- [Installation](#installation)
- [Utilisation](#utilisation)
- [Ressources Nécessaires](#ressources-nécessaires)
- [Auteur](#auteur)

## Description du Projet

Le projet vise à fournir des informations détaillées sur les happy hours des bars à Toulouse, en passant par les étapes de collecte de données, analyse, visualisation et envoi de rapport par e-mail.

## Technologies Utilisées

- Python
- Pandas
- BeautifulSoup
- Requests
- Folium
- Geopy
- smtplib
- email.mime
- Jupyter Notebook (optionnel pour l'analyse interactive)

## Étapes du Projet

### Partie 1 : Extraction des Données

1. Scraper les informations nécessaires à partir du site Schlouk Map : [Schlouk Map Toulouse](https://www.schlouk-map.com/fr/cities/toulouse/happy-hour)
   - Nom du bar
   - Heures d'ouverture
   - URL de la page spécifique du bar (lien href)
   - Services disponibles (uniquement les services "oui")
   - Prix des boissons pendant et hors happy hour
2. Stocker les données extraites dans un DataFrame pandas.

### Partie 2 : Analyse des Données

1. Analyser les prix des différents bars pour identifier les cinq bars proposant les meilleurs deals durant les happy hours.

### Partie 3 : Rapport par E-mail

1. Suivre le tutoriel de Mailtrap pour configurer l'envoi d'e-mails avec Python : [Mailtrap Blog](https://mailtrap.io/blog/python-send-email/)
   - Configurer l'envoi d'e-mails grâce à la bibliothèque `smtplib` et `email.mime`.
   - Préparer un e-mail au format HTML incluant le top 5 des meilleurs deals en happy hour à Toulouse, établi à partir des analyses effectuées.

### Partie 4 : Cartographie (Bonus)

1. Utiliser Leaflet pour créer une carte interactive des bars :
   - Récupérer les données de localisation de chaque bar pour afficher leur position sur la carte.
   - Marquer chaque bar avec des détails comme le nom, les horaires d'happy hour, et les prix.

## Installation

1. Clonez le dépôt :
   ```bash
   git clone https://github.com/votre-utilisateur/projet-happy-hours-toulouse.git
   cd projet-happy-hours-toulouse
   
## Ressources Nécessaires
Compte Mailtrap pour tester l'envoi d'e-mails : Mailtrap
Clé API pour le géocodage avec Geopy (facultatif mais recommandé pour de meilleures performances)

## Auteur 
Étudiant en Data Science
damien.lauger.edu@groupe-gema.com
