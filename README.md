# PokeApi 2.0.0

PokeApi est un projet codé sous ReactJS dont sa version inférieur la 1.0.0 à été faite sous Webpack et JS.
Cette version comporte toute les modifications et les remarques faite précédemment lors de la revue.

## Installation

Extraire l'archive contenant notre code source , et faire ceci :

```npm
npm install
```
Cela installera tout le nécessaire pour lancer le projet (ici node_modules).

Ensuite pour lancer notre application il suffira de faire :
```npm
npm start
```
Cela exécutera un serveur où la compilation et le lancement du site se fera automatiquement si l'on obtiens pas d'erreur.

Vous aurez aussi l'option de nettoyer le dossier 'dist' si vous rencontrez un problème.
Taper juste :

```npm
npm run clean
```

## Explication des modifications

   1ere partie : POO
Il nous manquer dans notre projet la POO en soit une classe pour les pokemons pour rendre le code plus fluide.
Alors on a opter pour une classe pour :
- les pokemons --> "Pokemon.js"
- la carte d'un pokemon --> "PokemonCardDetails.js"
- une pour les détails des pokemons --> "PokemonDetails.js"
- pour lister la liste des pokemons --> "PokemonList.js"
- pour lister les types des pokemons --> "PokemonTypeList.js"


   2ieme partie : Dépendance d'images
Pour mieux gérer les dépendances d'images , on a donc décider de télécharger et mettre en local toutes les sprites (images) des pokemons, ainsi que le background (gif) en fond d'écran du site, etc...

Vous retrouverez dans le dossier 'assets/images' toutes les images utilisés pour gérer les dépendances avec la configuration Webpack requise.

   
   3ieme partie : Transpilage type Babel
Suite à la remarque on a directement implémenter Babel pour l'utilisation de l'ES6.
(voir la config webpack , et le package.json)


   4ieme partie : Asynchrone , fonction flèches
Pour cette partie on a donc adapté nos fonctions de départ et les a donc retransformés pour l'utilisation des callbacks , fonctions asynchrone , et les fonctions flèches.

Au début du projet on avait opter pour l'utilisation de Axios et/ou Xhr mais finalement on a opter pour fetch , on a remarque que leurs utilisation était plus apprécier (moins d'erreur) pour notre méthode implémentation et lors des tests sur l'API.


   5ieme partie : le CSS
Pour cette partie ce n'étais pas une remarque qui à été faite mais j'aimerai en parler , on a revue pas mal de chose au niveau du style à la fin du projet , comme l'utilisation du sccs très pratique d'utilisation.

Au niveau de la présentation du site on a laissé la recherche de type de pokemon mais on a enlevé la recherche de baies ou de pokemon via une barre de recherche.
On a remplacer ceci par l'utilisation du site plus fluide et plus dynamiques (avec du bootstrap).


## Contributing
Johan BOSQUET et Dorian CLOCHE

## License
2020
