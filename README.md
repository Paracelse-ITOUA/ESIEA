# Projet 1 DevOps - Groupe 6 
 - Convention de nommage :
feature/NOM
fix/ERROR
docs/DOCUMENT
test/NOM_DU_TEST

- Conflit créer par la modification simultané d'un fichier par deux utilisateurs différents sur 2 branches, confilt résolu en éditant le 
fichier et en supprimant les marqueurs
MAJOR.MINOR.PATCH : MAJOR = breaking change, MINOR = feature
test
test-2
test-3

# Projet 2 DevOps - Seul

[![CI](https://github.com/Paracelse-ITOUA/ESIEA/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/Paracelse-ITOUA/ESIEA/actions/workflows/ci.yml)

Projet réalisé en septembre 2026.

## Application

L'application de démonstration se trouve dans `starter-app/`.

Elle utilise :

- Python
- Flask
- pytest
- pytest-cov
- flake8

## Tests locaux

Créer et activer un environnement virtuel :

```bash
cd starter-app

python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt

# Conteneurisation Docker

## Construction de l'image

L'application Flask est construite avec un Dockerfile multi-stage.

```bash
docker build -t esiea-flask:multistage ./starter-app