JAVA :
static
final
transian
synchronysed
interface 
class abstraite
singleton
pattern strategy


JS/AngularJS : 
directive
DOM

# Chose à savoir en JAVA

## Static

On appelle élément statique d'une classe tout élément attaché à cette classe plutôt qu'à l'une de ses instances. Un élément statique peut exister, être référencé, ou s'exécuter même si aucune instance de cette classe n'existe.

Il est possible de définir quatre types d'éléments statiques :

* des champs statiques : la valeur de ce champ est la même pour tous les objets instance de la classe ;
* des méthodes statiques ;
* des blocs statiques ;
* des classes membre statiques.

## Final

De manière général, un élément final ne peut plus être modifié lors de l'execution du programme. 

Il est possible de définir le trois types déléments finaux.

* des champs : le champs devient constant donc la valeur ne peut pas être modifiée.
* des méthodes : la méthode ne peut pas être surchargée.
* des classes : la classe ne peux pas hériter.

## Classe abstraite

Une classe abstraite est une classe sans objet autrement dit elle ne peux pas être instanciée.
De plus elle doit contenir au moins une methode abstraite. En claire elle insite à l'extention et la surcharge de methode.

## Interface

Une interface est semblable a une classe abstraite avec quelque différence. Elle permet notament de régler le problème de l'héritage
multiple.

Une interface :

* possède que des méthode abstraites.
* ne peux pas être instanciée.
* peut possèder que des constantes (cham.ps finaux).
* une  peux etendre une autre interface.
* une classe peut étendre une ou plusieurs interfaces.

## Transient

Le mot-clé transient (éphémère ou transitoire) est lié à la sérialisation des classes Java. Il permet d'interdire la sérialisation de certaines variables d'une classe.

## Sérialisation

Sérializer un objet consiste à le convertir en un tableau d'octets, que l'on peut ensuite écrire dans un fichier, envoyer sur un réseau au travers d'une socket etc... Ce mécanisme existe depuis les débuts de l'API Java I/O, et il est très pratique. Il suffit de passer tout objet qui implémente l'interface Serializable à une instance de ObjectOutputStream pour sérialiser un objet.

Exemple : http://blog.paumard.org/cours/java/chap10-entrees-sorties-serialization.html

## Synchronized

blabla...

## Design Pattern

Un patron de conception autrement dit une bonne pratique permettant de résoudre un problème de conception logiciel.

### Singleton 

Il s’agit d’une classe qui ne peut posséder qu’une unique instance et offre un accès universel à cette instance.

Exemple : http://blog.paumard.org/2011/04/22/bilan-sur-le-pattern-singleton/ ou
          http://thecodersbreakfast.net/index.php?post/2008/02/25/26-de-la-bonne-implementation-du-singleton-en-java
          


### Strategy

Ajouter à la classe une méthode ayant en paramètre un algorithme (sous forme d’expression lamda ou d’objet). En claire gérer 
des comportements dynamiquement.







