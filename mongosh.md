# Tutoriel de prise en main de Mongosh87
## Introduction:
Mongosh est un shell interactif puissant pour MongoDB qui offre une expérience de développement améliorée. Dans ce tutoriel, nous vous guiderons à travers les étapes pour prendre en main Mongosh en utilisant uniquement la ligne de commande. Vous apprendrez comment installer Mongosh, vous connecter à votre base de données MongoDB et effectuer des opérations courantes en utilisant les commandes CLI.

## Étape 1: Installation de Mongosh
La première étape consiste à installer Mongosh sur votre machine. Mongosh est disponible en tant que package CLI, ce qui facilite son installation et son utilisation. Vous pouvez visiter le site officiel de Mongosh (https://www.mongodb.com/products/shell) pour télécharger le package approprié en fonction de votre système d'exploitation. Suivez les instructions spécifiques à votre système pour terminer l'installation.

## Étape 2: Connexion à votre base de données MongoDB
Une fois Mongosh installé, ouvrez une nouvelle fenêtre de terminal et exécutez la commande "mongosh". Par défaut, Mongosh se connectera à une instance MongoDB locale en utilisant les paramètres par défaut. Si vous souhaitez vous connecter à une autre instance MongoDB distante, vous pouvez spécifier l'URL de connexion en utilisant l'option "--host" lors de l'exécution de la commande mongosh.

```css 
mongosh --host <URL_de_connexion>
```

## Étape 3: Exploration de votre base de données
Maintenant que vous êtes connecté à votre base de données MongoDB, vous pouvez commencer à explorer et à interagir avec vos collections de données en utilisant des commandes CLI. Voici quelques commandes couramment utilisées :

Pour afficher toutes les bases de données :

```sql 
show databases
```

Pour sélectionner une base de données spécifique :

```perl 
use <nom_de_la_base_de_données>
```

Pour afficher les collections dans une base de données :

```sql
show collections
```

Pour afficher les documents d'une collection :

```lua
db.<nom_de_la_collection>.find()
```

Pour insérer un nouveau document dans une collection :

```php
db.<nom_de_la_collection>.insertOne({<champs>})
```

## Étape 4: Opérations avancées avec Mongosh CLI
Mongosh CLI offre également des fonctionnalités avancées pour effectuer des opérations plus complexes. Par exemple, vous pouvez utiliser la méthode "updateOne" pour mettre à jour un document existant, la méthode "deleteOne" pour supprimer un document, et la méthode "aggregate" pour effectuer des agrégations de données.

Voici un exemple d'utilisation de la méthode "updateOne" pour mettre à jour un document :

```php
db.<nom_de_la_collection>.updateOne({<filtre>}, {$set: {<champs>}})
```

## Conclusion
Dans ce tutoriel, nous avons appris à utiliser Mongosh en utilisant uniquement la ligne de commande. Vous avez appris comment installer Mongosh, vous connecter à votre base de données MongoDB et effectuer des opérations courantes en utilisant les commandes CLI. Avec Mongosh CLI, vous disposez d'un outil puissant pour interagir avec MongoDB et gérer efficacement vos données.
