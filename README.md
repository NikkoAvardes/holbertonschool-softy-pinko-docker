# Softy Pinko Docker

Projet d'apprentissage de Docker avec une application web full-stack.

## 📋 Description

Ce projet démontre la conteneurisation d'une application web moderne composée de :
- **Frontend** : Site web statique Softy Pinko servi par Nginx
- **Backend** : API REST Flask
- **Proxy** : Reverse proxy Nginx pour router les requêtes

## 🗂️ Structure

```
├── task0/          # Introduction à Docker
├── task1/          # Premier conteneur Flask
├── task2/          # Architecture front-end + back-end
├── task3/          # Optimisation des conteneurs
├── task4/          # Docker Compose
├── task5/          # Ajout du reverse proxy
├── task6/          # Load balancing et scaling
```

## 🚀 Démarrage rapide

### Prérequis
- Docker
- Docker Compose

### Lancer l'application (task6)

```bash
cd task6
docker-compose up -d
```

L'application sera accessible sur `http://localhost`

### Arrêter l'application

```bash
docker-compose down
```

## 🧪 Tests

Une suite complète de tests est disponible dans le dossier [tests/](tests/).

```bash
cd tests
./run_all_tests.sh
```

Voir [tests/README.md](tests/README.md) pour plus de détails.

## 📦 Services

| Service | Port | Description |
|---------|------|-------------|
| Proxy | 80 | Reverse proxy Nginx |
| Frontend | 9000 | Interface web |
| Backend | 5252 | API REST Flask |

## 🛠️ Commandes utiles

```bash
# Voir les conteneurs en cours d'exécution
docker-compose ps

# Voir les logs
docker-compose logs -f

# Reconstruire les images
docker-compose build

# Nettoyer tout
docker-compose down -v
```

## 📝 Notes

Ce projet fait partie du cursus Holberton School pour l'apprentissage de Docker et de l'orchestration de conteneurs.