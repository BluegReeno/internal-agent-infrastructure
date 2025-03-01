# Infrastructure d'Agents IA BG

Une plateforme modulaire pour le développement rapide d'agents IA spécialisés pour Blue Green, s'appuyant sur Claude 3.7 Sonnet.

## 🌟 Vision

Cette infrastructure vise à standardiser et accélérer le développement d'agents IA chez Blue Green. Conçue spécifiquement pour les besoins du secteur des énergies renouvelables, elle permet de créer rapidement des agents capables d'extraire, d'analyser et d'exploiter des informations techniques pour améliorer l'efficacité opérationnelle.

## 🏗️ Architecture

L'infrastructure s'appuie sur ces composants clés :

- **Base de connaissances** : Instance Supabase dédiée pour le stockage et la récupération vectorielle des documentations techniques
- **Extraction documentaire** : Intégration de crawl4ai pour l'acquisition automatique de documentations
- **Traitement PDF** : Module basé sur doclin pour l'extraction structurée des données à partir de documents PDF
- **Modèle principal** : Claude 3.7 Sonnet
- **Vectorisation** : Service d'embedding pour la recherche sémantique (Voyager AI envisagé)
- **Orchestration** : Intégration n8n pour l'automatisation des flux de travail

## 🚀 Fonctionnalités principales

- Extraction et indexation automatique de documentations techniques
- Traitement intelligent des documents PDF et extraction structurée
- Base de connaissances vectorielle dans Supabase avec récupération sémantique
- Raisonnement via prompting de Claude 3.7 Sonnet
- Orchestration des flux de travail avec n8n
- Gestion du contexte et de la mémoire des conversations

## 📊 Métadonnées des outils

Chaque outil intégré dans l'infrastructure est caractérisé par un schéma de métadonnées standardisé :

- Identifiant unique et version
- Fonctionnalités principales et cas d'usage
- Paramètres d'entrée/sortie et contraintes
- Documentation de référence et exemples
- Dépendances et compatibilités

## 🔧 Installation

```bash
# Cloner le repository
git clone https://github.com/bluegreen-ai/internal-agent-infrastructure.git
cd internal-agent-infrastructure

# Installer les dépendances
pip install -r requirements.txt

# Configurer les variables d'environnement
cp .env.example .env
# Éditer le fichier .env avec vos clés API et configurations
```

## 🔒 Sécurité et gestion des APIs

Ce projet utilise plusieurs services externes nécessitant des clés API :

- Claude 3.7 Sonnet (Anthropic)
- Service d'embedding (Voyager AI envisagé)
- Supabase
- Crawl4AI

Les clés API seront stockées dans le fichier .env qui est ajouté au .gitignore pour éviter tout partage accidentel.

## 🤝 Contribution

Ce projet est réservé à l'usage interne de Blue Green. Pour contribuer :

1. Créez une branche pour votre fonctionnalité (`git checkout -b feature/amazing-feature`)
2. Committez vos changements (`git commit -m 'Add some amazing feature'`)
3. Poussez vers la branche (`git push origin feature/amazing-feature`)
4. Ouvrez une Pull Request

## 📝 Licence

Usage interne uniquement. Copyright © 2025 Blue Green.