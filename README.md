# Hospital Information System for Gastroenterology (ICD-11 Integration)

## Description

Ce projet consiste en le développement d'un système d'information hospitalier (SIH) pour le service de gastroentérologie, intégrant la classification internationale des maladies (ICD-11). L'objectif principal est de faciliter la transition de l'ICD-10 vers l'ICD-11, tout en assurant une gestion efficace et sécurisée des dossiers médicaux électroniques (EHR).

## Objectifs du projet

- Remplacer l'ICD-10 par l'ICD-11 pour améliorer la précision et la spécificité des diagnostics.
- Permettre aux médecins de rechercher rapidement les codes ICD-11.
- Garantir la sécurité et la confidentialité des données médicales.
- Faciliter l'intégration avec les systèmes de gestion existants.

## Fonctionnalités principales

1. **Recherche et consultation des codes ICD-11 :**

   - Recherche en temps réel avec suggestions automatiques.
   - Affichage clair des résultats de recherche.
   - Ajout direct des codes sélectionnés dans les dossiers patients.

2. **Mise à jour des dossiers médicaux :**

   - Association des diagnostics ICD-11 aux patients.
   - Modification et suppression des diagnostics.
   - Archivage automatique des modifications.

3. **Gestion des utilisateurs et des rôles :**

   - Authentification sécurisée via JSON Web Tokens (JWT).
   - Gestion des rôles : administrateurs, médecins, patients.
   - Contrôle des permissions d'accès.

4. **Archivage des consultations :**

   - Sauvegarde automatique des consultations dans des fichiers CSV.
   - Recherche et consultation de l'historique médical.

## Technologies utilisées

### Backend

- **Django :** Framework web principal pour le backend.
- **Django Rest Framework :** API REST pour l'accès aux données.
- **SQLite :** Base de données légère pour le stockage local.
- **JSON Web Token (JWT) :** Authentification sécurisée.

### Frontend

- **HTML, CSS, Bootstrap :** Interface utilisateur intuitive et réactive.
- **AJAX :** Mise à jour dynamique des données sans rechargement de la page.

### Autres

- **Python & Pandas :** Manipulation des données médicales et des fichiers CSV.
- **StarUML :** Création des diagrammes UML pour la modélisation du système.

## Installation

1. Clonez le dépôt GitHub :
   ```bash
   git clone https://github.com/ton-utilisateur/ICD-11-Gastro-SIH.git
   ```
2. Accédez au répertoire du projet :
   ```bash
   cd ICD-11-Gastro-SIH
   ```
3. Installez les dépendances Python :
   ```bash
   pip install -r requirements.txt
   ```
4. Appliquez les migrations pour configurer la base de données :
   ```bash
   python manage.py migrate
   ```
5. Lancez le serveur de développement local :
   ```bash
   python manage.py runserver
   ```
6. Accédez à l'application via votre navigateur à l'adresse : `http://127.0.0.1:8000`

## Diagrammes UML

Des diagrammes UML ont été utilisés pour modéliser le système :

- **Diagramme de cas d'utilisation :** Montre les interactions entre les utilisateurs (administrateurs, médecins, patients) et les fonctionnalités principales.
- **Diagramme de classes :** Représente la structure des données et les relations entre les entités principales (patients, médecins, consultations, etc.).

Ces diagrammes sont disponibles dans le dossier `docs/`.

## Fichiers importants

- `src/` : Contient le code source de l'application.
- `data/icd11_dataset_clean.csv` : Base de données locale des codes ICD-11.
- `docs/` : Documentation et diagrammes UML.
- `requirements.txt` : Liste des dépendances Python.

## Sécurité

- Toutes les communications sont sécurisées via HTTPS.
- Les données sensibles sont protégées grâce au chiffrement et à une gestion stricte des permissions.
- Sauvegardes régulières des données pour prévenir toute perte.

## Contributeur

- **Majd Saadouli**



## Remerciements

Ce projet a été réalisé dans le cadre d'un stage technicien au Centre Informatique du Ministère de la Santé (CIMS),  un grand merci à toutes les personnes qui ont contribué à cette expérience enrichissante.

