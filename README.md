# CSHARP C#

## Créer une application en ligne de commande

````cmd
dotnet new console -o FirstApp
````
Resultat: 
````cmd

Bienvenue dans .NET 8.0 !
---------------------
Version du kit SDK : 8.0.401

Télémétrie
---------
Les outils .NET collectent des données d'utilisation qui nous aident à améliorer votre expérience utilisateur. Elles sont collectées par Microsoft et partagées par la communauté. Vous pouvez refuser l'adhésion à la télémétrie en affectant la valeur '1' ou 'true' à la variable d'environnement DOTNET_CLI_TELEMETRY_OPTOUT via l'interpréteur de commandes de votre choix.

Pour plus d'informations sur la télémétrie des outils CLI .NET, accédez à https://aka.ms/dotnet-cli-telemetry

----------------
Installation d'un certificat de développement HTTPS ASP.NET Core.
Pour faire confiance au certificat, exécutez 'dotnet dev-certs https --trust'
En savoir plus sur HTTPS : https://aka.ms/dotnet-https

----------------
écrivez votre première application : https://aka.ms/dotnet-hello-world
Découvrez les nouveautés : https://aka.ms/dotnet-whats-new
Explorez la documentation : https://aka.ms/dotnet-docs
signaler les problèmes et trouver une source sur GitHub : https://github.com/dotnet/core
Utilisez « dotnet --help » pour afficher les commandes disponibles ou visitez : https://aka.ms/dotnet-cli
--------------------------------------------------------------------------------------
Le modèle « Application console » a bien été créé.

Traitement des actions postérieures à la création en cours... Merci de patienter.
Restauration de C:\Users\afourmault\Documents\dev\csharp\csharp\FirstApp\FirstApp.csproj :
  Identification des projets à restaurer...
  Restauration effectuée de C:\Users\afourmault\Documents\dev\csharp\csharp\FirstApp\FirstApp.csproj (en 113 ms).
Restauration réussie.
````

fichier Program.cs

En c#, il est obligé davoir une methode Main pour lancer un programme
````c#
using System;

class Program // class
{
    static void Main(string[] args) // Methode
    {
        Console.WriteLine("Hello, World!");
    }
}
````

### build un projet

````cmd
dotnet build
````

va créer le projet avec l'executable

La commande dotnet run permet d'executer le programme
````cmd
dotnet run
````

Resultat
````cmd
Hello World!
````

### Déployer une application

commande pour plubier et créer le dossier publish pour avoir l'executable final
````cmd
dotnet publish
````

## Afficher du texte

````c#
Console.WriteLine("Hello, World!"); // écrit et passe à la ligne
Console.Write("Hello, World!"); // écrit sans passé à la ligne
Console.Beep(); //génére un BIP sonore
````


## Les variables

déclaration des variables en C#

````C#
//entié
int n = 0;
Console.WriteLine(n);
// chaine de caractère
string name = "Jason";
````

On peut convertire certain type en d'autre par exemple, un float en int
````C#
float number = 3.14f;
int nb = 0;
nb = (int)number;
````

Pour les grand nombre, pour que se soit plus lisible, il est possible de mettre un _ pour avoir une meilleure lisibilité

````C#
int nb = 2456784;
int nb = 2_456_784;
````

## Les opérateurs


