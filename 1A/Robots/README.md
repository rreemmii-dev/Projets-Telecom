# Robots

L'objectif de ce projet est de créer une flotte de robots se déplaçant de manière coordonnée afin de scanner des QR codes.
Chaque groupe est constitué de 5 robots.
Chaque robot est réalisé par une équipe de 4 étudiants, soit un total de 20 étudiants par groupe.

Le projet est constitué de deux phases : une première durant laquelle chaque équipe travaille individuellement sur son robot, puis une seconde durant laquelle les robots doivent se coordonner et communiquer entre eux.

Le langage de programmation utilisé était Python, notamment pour sa facilité d'utilisation.

<div align="center">
Notre robot avant / après décoration :
<br>
<img src="Avant.jpg" alt="Avant" width="45%" /> <img src="Après.jpg" alt="Après" width="45%" />
</div>


## Table des matières

* [Tâches à réaliser](#tâches-à-réaliser)
* [Organisation](#organisation)
* [Apprentissages](#apprentissages)


## Tâches à réaliser


### Organisation

La première étape est de définir une organisation pour l'équipe. Dans notre cas, chacune des tâches à réaliser s'est vue attribuer 1 ou 2 étudiants pour travailler dessus.

### Fabrication du robot

Le matériel de départ (batterie, roues, caméra) est fourni.
Il faut cependant fabriquer la carrosserie, tout assembler / brancher, et enfin décorer le robot.

### Contrôle des moteurs

Afin de contrôler le robot, il est nécessaire de contrôler les moteurs avec précision.
Nous avons donc implémenté un système d'asservissement mesurant la distance parcourue après chaque action et la comparant à la distance théorique.
Ainsi, le robot connaissait en permanence sa position théorique, mais aussi sa position réelle.

### Communication entre le site web et le robot

En plus du mode "conduite autonome", le robot doit pouvoir être contrôlé depuis un site web.
Il faut donc créer ce site web et l'interfacer avec les fonctions existantes permettant de contrôler le robot.

### Détection des QR codes

Bien qu'il existe des librairies permettant de détecter des QR codes, il est nécessaire de calibrer la caméra et de régler certains problèmes de luminosité afin que tout fonctionne correctement.

### Coordination entre robots

Une fois la deuxième phase commencée, les 5 robots doivent se coordonner entre eux.
Cela a nécessité la définition d'une stratégie de groupe et d'une convention pour la communication entre les robots.
L'objectif étant de scanner le plus de QR codes possibles au total des 5 robots, nos robots partageaient en continu aux autres robots la position des QR codes trouvés.


## Organisation

Une séance de 3h était prévue chaque semaine pour avancer sur le projet.

Durant la première phase, l'organisation et le travail de chaque équipe est indépendant : aucun partage d'information ou de code n'est autorisé entre les équipes.
A l'intérieur de mon groupe de 4, nous avions mis en place un fichier de suivi dans lequel chaque personne écrivait à la fin de la séance ce sur quoi elle avait travaillé.
Un planning établi au préalable permettait également de déterminer lorsqu'il était nécessaire de travailler chez soi en plus des séances prévues.
Enfin, la forte diversité dans le nombre de tâches à effectuer a permis à chaque personne de travailler sur un sujet différent.


## Apprentissages

La principale difficulté de ce projet a été l'organisation : le projet est long, avec de nombreuses parties indépendantes.
Notre méthode d'avoir chaque membre de l'équipe travaillant sur un sujet différent a permis d'avancer sur plusieurs fronts à la fois.
Cependant, il est arrivé que des membres en difficulté travaillant seuls ne demandent pas d'aide, préférant mettre les problèmes sous le tapis.
Il aurait donc été pertinent de prendre plus de temps pour faire des comptes-rendus des avancées de chacun en fin de séance, au lieu de simplement dire "X avance sur Y".

De plus, l'absence de planning global entre les équipes du groupe s'est ressentie : certaines équipes ont fini de travailler sur leur robot avant d'autres, les empêchant de commencer la deuxième phase.

Pour finir, voici l'affiche de présentation de notre robot :

<div align="center">
<img src="Affiche.png" alt="Affiche" width="75%" />
</div>
