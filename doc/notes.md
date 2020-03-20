# Notes sur le projet

L'objectif est de faire un bot sur le Discord qui permettrait de simplement de jouer de la musique au plus grand des calmes dans les différents salons du foyer virtuel. Le fait est que cela existe déjà, et que quitte à réinventer la roue, autant fork un projet d'un de ces bots et le modifier pour l'adapter à nos besoins.

Il serait peut-être mieux de faire un bot qui puisse s'interfacer avec Spotify, et qui permettrait aux membres du foyer Reddit d'accéder aux différents playlists de TSM (pas encore créées), et d'éventuellement faire en sorte que le bot lise en permanence des morceaux sur Spotify, afin que les gens puissent rejoindre ce qu'écoute le bot en live (ça fera un genre de radio stream assez sympa). 

Pour créer un bot, Discord met à disposition une bibliothèque bien documentée, *discord.py* qui permet de connecter le bot au serveur que l'on souhaite, et de pouvoir interagir avec le serveur.

On peut ensuite coller derrière ce bot une autre bibliothèque python destinée à créer un chat bot, et qui, à partir des messages envoyés par les utilisateurs, peut effectuer des actions (en l'occurence, inviter à écouter une playlist, ou inviter à rejoindre le stream).

Finalement, Spotify est bien intégré à Discord, donc on pourrait être bien parti pour faire un beau petit bot DJ.

## Fonctionnalités qu'on voulait qui ne vont pas marcher

En fait non. Créer un bot semble pouvoir bien se faire grâce aux différentes biblothèques / API / docs qu'on peut trouver en ligne. Par contre, la partie "interface" entre Spotify, le bot et Discord semble être largement compromise :

* C'est quelque peu illégal de faire tourner un bot en continu sur Spotify 
* Il n'existe pas de manière d'inviter des gens à écouter une certaine musique sur Spotify en ligne de commandes, ou de les inviter à rejoindre le stream.

Bref, le projet semble quelque peu compromis :'( 
