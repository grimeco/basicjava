# Basilic
Le langage Basilic est un langage procédural visant à offrir une syntaxe simple analogue à celle du langage Basic, mais permettant d’exploiter toutes les ressources disponibles dans le langage Java. Basilic est implanté comme un langage de script. Un « compilateur » traduit le code basilic en code java.

La documentation est disponible sur le site [grimeco](https://grimeco.fr)

## Exemple: 
fichier helloworld.bcj
```
println("Helloworld")
```
helloworld.java : code java produit par le « compilateur »
```
public class helloworld 
  {
   public static void main(String[]args)
    {
     cbsystem.setArgs(args);
     new helloworld();
    }

   helloworld()
   {
    cbconsole.println(new cbstring("Hello world!"));
   }
  }
```
Basilic est un langage très fortement typé. Aucune conversion implicite n’est autorisée.

Basilic est modulaire. Une unité de compilation (fichier source) correspond à une classe Java. Il n’y a pas de type primitif tel que char, int ,…

Il suffit de définir pour chaque type primitif un module réalisant l’implémentation correspondante.

La version minimale de Basilic est fournie avec les modules (classes) suivants:

boolean, int, string, double, long, byte, system, console, stringvector, conversions, lexical, datetime, filedirectory, inifile, arraytools, stringhashmap, stringstack et zip

Ces modules permettent notamment de modifier et de recompiler le compilateur Basilic si l’on souhaite y apporter des modifications.

## Pourquoi Basilic ?

Aucune raison logique !

Peut-être une référence à la chambre des secrets dans Harry Potter ?

et le langage Python ?

# Basilic
The Basilic language is a procedural language aiming to offer a simple syntax similar to that of the Basic language, but making it possible to exploit all the resources available in the Java language. Basilic is implemented as a scripting language. A "compiler" translates basilic code into java code. 

The documentation is available on the [grimeco](https://grimeco.fr) website
## Example: 
file helloworld.bcj
```
println("Helloworld")
```
file helloworld.java : java code produced by the “compiler”
```
public class helloworld 
  {
   public static void main(String[]args)
    {
     cbsystem.setArgs(args);
     new helloworld();
    }

   helloworld()
   {
    cbconsole.println(new cbstring("Hello world!"));
   }
  }
```
Basilic is a very strongly typed language. No implicit conversion is allowed.

Basilic is modular. A compilation unit (source file) corresponds to a Java class. There is no primitive type such as char, int,…

It suffices to define for each primitive type a module realizing the corresponding implementation.

The minimum version of Basiluc comes with the following modules (class):

boolean, int, string, double, long, byte, system, console, stringvector, conversions, lexical, datetime, filedirectory, inifile, arraytools, stringhashmap, stringstack and zip

These modules allow you to modify and recompile the Basilic compiler if you want to make changes to it.
## Why Basilic?

No logical reason!

Perhaps a reference to the Chamber of Secrets in Harry Potter?

and the Python language?
## Version 1.0, 15 mai 2022
