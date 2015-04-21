# Étape 2 - Travail à réaliser

Bonjour !
Voici le site que j'ai réalisé pour la 4ème étape des travaux à réaliser.
C'est le travail qui a monopolisé l'extrême majorité de mon temps.

## Apprentissage du CSS et de l'HTML

Quand j'ai reçu le mail indiquant les exercices à rendre, j'ai décidé de me concentrer sur le quatrième car il était dans la ligné de ce que j'étais en train d'étudier. J'avais commencé à étudier le webdesign sur [ce site](http://www.steaw-webdesign.com/css/~).

## Contributions

Les articles peuvent être postés ici sous forme de PR une fois qu'on est OK dans [une
issue du repo](https://github.com/putaindecode/putaindecode.fr/issues).
Si vous souhaitez voir un post écrit, ou même en écrire un, faites un tour là bas ;)

Pour contribuer au site, n'hésitez pas, en plus de lire la partie technique ci-dessous,
à lire le fichier spécifique [CONTRIBUTING.md](CONTRIBUTING.md)

---

## Développement

__Notice: Faites attention à la configuration de vos éditeurs de texte et IDE.  
Nous utilisons [`.editorconfig`](.editorconfig) pour garder une cohérence.
Respectez cela (il vous suffit d'aller sur le site [editorconfig.org/](http://editorconfig.org/)
pour télécharger le plugin adéquat pour votre éditeur.__

Ce site utilise [gulp](https://github.com/gulpjs/gulp),
il vous est donc conseillé de jeter un coup d'oeil au [README de gulp](https://github.com/gulpjs/gulp#readme)
avant d'intervenir sur le projet ;).

## Récupérer les sources du site

```console
$ git clone https://github.com/putaindecode/putaindecode.fr.git
$ cd website
$ npm run init
$ npm install
```

## Mettre à jour les sources

Lorsque vous n'avez pas travaillé sur le site depuis un petit moment, on vous conseille
d'exécuter les commandes suivantes :

```console
$ git pull
$ npm install
```

Si vous rencontrez des erreurs lors du `git pull` (par ex. pour une histoire de
fichiers modifiés non commités), vous pouvez juste avant faire
un petit

```console
$ git reset --hard
```

__Note: cela supprimera toutes vos modifications locales sans avertissement, à
faire avec précaution.
Préférez `git stash` si vous souhaitez conserver vos modifications__.

## Lancer le site web localement

```console
$ npm start
```

Oui oui, c'est tout, vous devriez avoir le site web qui s'ouvre tout seul dans votre navigateur.
Si ce n'est pas le cas, et que vous n'avez pas d'erreurs dans votre console,
rendez-vous à l'adresse suivante: [http://localhost:4242](http://localhost:4242).


## Mise en production

La commande suivante (lorsque vous avez les droits nécessaires) va construire le site
en version optimisée, et le publier (mise à jour de la branche  `gh-pages`, qui,
grâce à GitHub, suffit à mettre en ligne le site).

```console
$ npm run deploy
```

**Cela dit, tous les commits dans la branche `master` provoqueront une mise en production automatique via [Travis-CI](https://travis-ci.org/).**

_Note: pour commiter sans provoquer un `deploy`, il suffit d'ajouter `[ci skip]` dans votre message de commit._

---

## Mise à jour spécifiques

### Générer le favicon

Installez [icoutils](http://www.nongnu.org/icoutils/). Par exemple sur OS X :

```console
$ brew install icoutils
```

ou

```console
$ npm run init-osx
```

Ensuite utilisez la commande suivante

```console
$ npm run favicon
```

---

## Crédits

### Auteurs et contributeurs

* [Membres de l'organisation](https://github.com/putaindecode?tab=members)
* [Liste des contributeurs](https://github.com/putaindecode/putaindecode.fr/graphs/contributors)

### Logo & Avatar

Remerciements à toutes les personnes impliquées dans cette discussion [putaindecode/organisation/issues/4](https://github.com/putaindecode/organisation/issues/4).
Remerciement spécial à [@bloodyowl](https://github.com/bloodyowl) pour le [logo initial](https://github.com/putaindecode/putaindecode.fr/blob/3324cbe7637dacd1f42a412c1085431a2d551928/src/assets/_images/p!-logos.png).
