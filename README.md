# Infrastructure d'Agents IA BG

Une plateforme modulaire pour le développement rapide d'agents IA spécialisés pour Blue Green, basée sur [Archon](https://github.com/coleam00/Archon) et utilisant Claude 3.7 Sonnet.

## 🌟 Vision

Cette infrastructure vise à standardiser et accélérer le développement d'agents IA chez Blue Green. Conçue spécifiquement pour les besoins du secteur des énergies renouvelables, elle permet de créer rapidement des agents capables d'extraire, d'analyser et d'exploiter des informations techniques pour améliorer l'efficacité opérationnelle.

## 🏗️ Architecture

Ce projet est un **fork d'Archon** enrichi avec des fonctionnalités spécifiques pour Blue Green. L'infrastructure s'appuie sur ces composants clés :

- **Base de connaissances** : Instance Supabase dédiée pour le stockage et la récupération vectorielle
- **Extraction documentaire** : Intégration de crawl4ai (installé localement) pour l'acquisition automatique de documentations
- **Modèle principal** : Claude 3.7 Sonnet
- **Vectorisation** : Service d'embedding pour la recherche sémantique
- **Orchestration** : Intégration n8n pour l'automatisation des flux de travail
- **Intégration Notion** : Synchronisation avec le QG Blue Green pour la gestion des tâches

## 🚀 Fonctionnalités principales

- Extraction et indexation automatique de documentations techniques
- Base de connaissances vectorielle dans Supabase avec récupération sémantique
- Raisonnement via prompting de Claude 3.7 Sonnet
- Orchestration des flux de travail avec n8n
- Gestion du contexte et de la mémoire des conversations
- Synchronisation avec GitHub et Notion

## 🔧 Installation

```bash
# Cloner le repository
git clone https://github.com/bluegreen-ai/internal-agent-infrastructure.git
cd internal-agent-infrastructure

# Déploiement Docker (recommandé)
python run_docker.py

# Configurer les variables d'environnement
cp .env.example .env
# Éditer le fichier .env avec vos clés API et configurations
```

## 🔒 Sécurité et gestion des APIs

Ce projet utilise plusieurs services externes nécessitant des clés API :

- Claude 3.7 Sonnet (Anthropic)
- Service d'embedding
- Supabase
- Crawl4AI (installé localement)

Les clés API sont stockées dans le fichier .env qui est ajouté au .gitignore pour éviter tout partage accidentel.

## 🔄 Synchronisation avec Archon

Ce projet est un fork d'[Archon](https://github.com/coleam00/Archon) et nous prévoyons d'intégrer les améliorations futures (v5 et au-delà) lorsqu'elles seront disponibles. Notre objectif est d'enrichir l'infrastructure d'Archon avec des fonctionnalités spécifiques pour le secteur des énergies renouvelables tout en bénéficiant des avancées de la communauté.

## 🤝 Contribution

Ce projet est réservé à l'usage interne de Blue Green. Pour contribuer :

1. Créez une branche pour votre fonctionnalité (`git checkout -b feature/amazing-feature`)
2. Committez vos changements (`git commit -m 'Add some amazing feature'`)
3. Poussez vers la branche (`git push origin feature/amazing-feature`)
4. Ouvrez une Pull Request

## 📝 Licence

Usage interne uniquement. Copyright © 2025 Blue Green.