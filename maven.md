# Maven

<h2>Intro</h2>

Maven est un outil de construction de projets (build) open source développé par la fondation Apache. Il permet de faciliter et d'automatiser certaines tâches de la gestion d'un projet Java.

Pour assurer la construction d'un projet, Maven propose notamment de prendre en charge :

* La compilation
* Le packaging
* La gestion des dépendances
* La génération de la documentation
* L'accès au gestionnaire de sources
* L'accès aux dépôts ou aux gestionnaires de dépendances
* Le déploiement
* ... et de très nombreuses autres tâches requises lors d'un build

  <h3>Gestion des dépendances</h3>

  Maven permet de gérer les dépendances d'un projet en configurant le fichier pom.xml.

  * Les dépendances sont identifiées grâce aux informations : groupId, artifactId, version
  * Les dépendances peuvent être de plusieurs types : jar, zip, pom, ...

<h2>Plugin</h2>

Toutes les fonctionnalités de Maven sont proposées sous la forme de plugins.

<h2>POM.xml</h2>

Maven est orienté projet, donc le projet est l'entité principale gérée par Maven. Il est nécessaire de fournir à Maven une description du projet (Project descriptor) sous la forme d'un document XML nommé project.xml et situé à la racine du répertoire contenant le projet.

  <h3>Super POM</h3>

  Tous les projets Maven héritent d'un super POM
 
  Pour visualiser le super POM : 
  
  * Désarchiver le fichier M2_HOME/lib/maven-model-builder- 3.3.3.jar
  * Le super POM se trouve dans le fichier org/apache/maven/model/pom-4.0.0.xml
  * Il contient la configuration Maven par défaut => la convention Maven
  
  <h3>POM effectif</h3>
  
  * Les POMs héritent leur configuration d'autres POMs (à minima du super POM).
  * Le modèle objet du projet va au final être la combinaison des configurations (via le lien d'héritage)
  * Pour visualiser toute la configuration d'un POM mvn help:effective-pom

<h2>Un ensemble de conventions</h2>

Maven privilégie une approche "convention over configuration" :

* Les sources java sont supposés être dans le répertoire src/main/java
* Les autres fichiers nécessaire au programme (.properties, .xml) sont supposés être dans le répertoire src/main/resources
* Les sources java des tests sont sont supposés être dans le répertoire src/test/java
* Les autres fichiers nécessaire aux tests (.properties, .xml) sont supposés être dans lerépertoire src/test/resources
* Les fichiers générés par Maven sont dans le répertoire target
* Les fichiers web (html, css, jsp, ...) sont supposés être dans le répertoire src/main/webapp
