# Compilateur

Ce projet consistait à créer un compilateur C vers assembleur x86, en équipe de 4 étudiants.

Le langage de programmation retenu est OCaml.


## Table des matières

* [Tâches à réaliser](#tâches-à-réaliser)
* [Organisation](#organisation)
* [Apprentissages](#apprentissages)


## Tâches à réaliser

Différentes étapes sont nécessaires pour passer d'un code C à x86 :

### Lexing

La première étape consiste à transformer le texte en "tokens" ayant un sens.
Par exemple, `int x = 0;` se transforme en `type (int), name (x), equal, integer (0), semicolon`.

Pour cela, nous avons défini nos tokens et utilisé le module `Lexing` de OCaml.

### Parsing

L'étape suivante est de donner du sens aux tokens obtenus précédemment.
Par exemple, une assignation de variable est `type, name, equal, value, semicolon`, avec `value` pouvant être un token `integer` ou un autre (`char`, `expr` de la forme a + b, etc.)

Nous avons défini l'ensemble de notre arbre syntaxique grâce au module `Parser` de OCaml.

### Ecriture du code Assembleur

Une fois l'arbre syntaxique obtenu par le parsing, il ne reste plus qu'à le traduire en assembleur.

Nous avons donc dû étudier le fonctionnement de l'assembleur x86, et les diverses opérations et registres existants.


## Organisation

Le travail à réaliser lors de ce projet était relativement simple à paralléliser : le code était naturellement composé de plusieurs fonctions comme `compile_expr` (compile une expression telle que `a + b`) ou `compile_stmt` (compile un statement tel que `int x = 0;`).

L'organisation par défaut était donc de donner à chaque élève un certains nombre de fonctions à réaliser, puis de travailler en peer-programming lorsqu'un membre du groupe était en difficulté.


## Apprentissages

Ce projet a été mon premier projet en groupe réalisé à Télécom Paris.
En plus de m'apprendre le fonctionnement d'un ordinateur au plus bas niveau, il m'a permis de découvrir les difficultés liées aux travaux de groupes : différence de compétences et de motivation entre les membres du groupe, nécessité d'organiser le travail, etc.
