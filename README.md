# TOS_SolR

Bienvenue dans le référentiel de Votre Projet. Ce référentiel contient des informations sur l'installation et la configuration de Apache Solr pour votre application.

## Apache Solr

Apache Solr est une plateforme de recherche open source basée sur Lucene. Elle offre une recherche puissante et des fonctionnalités d'indexation pour vos données.

## Installation

Suivez ces étapes pour installer Solr localement :

1. **Téléchargement de Solr :**
   Téléchargez la dernière version de Solr depuis le [site officiel de Solr](https://lucene.apache.org/solr/downloads.html).

2. **Extraction des fichiers :**
   Extrayez les fichiers téléchargés dans le répertoire de votre choix.

3. **Configuration du noyau (Core) :**
   - Accédez au répertoire Solr que vous avez extrait.
   - Naviguez vers le répertoire `server/solr`.
   - Copiez le répertoire `configsets/_default` et renommez-le selon les besoins de votre application.
   - Modifiez le fichier `core.properties` dans le nouveau répertoire pour refléter le nom du core et les paramètres spécifiques de votre projet.

4. **Démarrage de Solr :**
   - Depuis le répertoire principal de Solr, exécutez la commande :
     ```bash
     bin/solr start
     ```

5. **Création du Core :**
   - Créez le core en utilisant la commande suivante (assurez-vous d'ajuster le chemin vers le répertoire core) :
     ```bash
     bin/solr create_core -c VOTRE_CORE -d chemin/vers/votre/configset
     ```

6. **Accès à l'interface d'administration :**
   - Ouvrez votre navigateur et accédez à [http://localhost:8983/solr/](http://localhost:8983/solr/) pour accéder à l'interface d'administration de Solr.

## Configuration Supplémentaire

- Pour personnaliser davantage la configuration de Solr, consultez la documentation officielle de Solr : [https://lucene.apache.org/solr/guide/](https://lucene.apache.org/solr/guide/).


Les contributions sont les bienvenues ! Si vous avez des suggestions d'amélioration, des rapports de bogues ou des fonctionnalités à ajouter, n'hésitez pas à ouvrir une issue ou à soumettre une pull request.

