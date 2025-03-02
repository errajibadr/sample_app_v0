# Application Web d'Exemple

Cette application web se compose d'une API backend et d'une interface frontend.

## Structure du Projet

.
├── api/

    ├── sample_api.py    # Implémentation de l'API backend
    ├── Dockerfile       # Configuration du conteneur API
    └── requirements.txt # Dépendances Python pour l'API

└── web_app/

    ├── ui.py           # Interface utilisateur frontend
    └── Dockerfile      # Configuration du conteneur web

## Fonctionnalités

- API REST backend
- Interface utilisateur web
- Support du déploiement conteneurisé
- Configuration simple pour le développement local

## Prérequis

- Python 3.8+
- Docker & Docker Compose (optionnel)
- Git

## Démarrage Rapide

### Développement Local

1. Cloner le dépôt :

    git clone <url-de-votre-repo>
    cd sample-web-app

2. Configurer l'API :

    cd api
    pip install -r requirements.txt
    python sample_api.py

3. Configurer l'interface web :

    cd web_app
    pip install -r requirements.txt
    python ui.py

### Déploiement avec Docker

Lancer les deux services avec Docker Compose :

    docker-compose up

## Points d'Accès API

- GET /api/health - Vérification de l'état
- GET /api/data - Récupération des données
- POST /api/data - Création d'une nouvelle entrée

## Accès aux Services

- API Backend : http://localhost:5000
- Interface Web : http://localhost:8000

## Contribution

1. Créez une branche (git checkout -b feature/nouvelle-fonctionnalite)
2. Committez vos changements (git commit -m 'Ajout d'une nouvelle fonctionnalité')
3. Poussez vers la branche (git push origin feature/nouvelle-fonctionnalite)
4. Ouvrez une Pull Request
