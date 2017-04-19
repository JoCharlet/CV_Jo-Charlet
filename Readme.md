# Projet création d'une page web Jonathan Charlet
[lien](app/apple-touch-icon.png)
Création d'un site web CV avec le framework Bootstrap en utilisant les outils de développement NPM, Yeoman, Bower, Gulp, Git et GitHub. La documentation de ce projet est écrite avec le langage de balisage markdown

**Table des matières**

1.  [Présentation des outils utilisés](#1-présentation-des-outils)
    - [1.1 Éditeur de code](#11-Éditeur-de-code)
 	- [1.2 HTML](#12-html)
	- [1.3 CSS](#13-css)
	- [1.4 JavaScript](#14-javascript)
	- [1.5 jQuery](#15-jquery)
	- [1.6 Bootstrap](#16-bootstrap)
	- [1.7 Modernizr](#17-modernizr)
	- [1.8 Node.js & npm](#18-nodejs--npm)
	- [1.9 Yeoman](#19-yeoman)
	- [1.10 Bower](#110-bower)
	- [1.11 Gulp](#111-gulp)
	- [1.12 Git](#112-git)
	- [1.13 GitHub](#113-github)
	- [1.14 Markdown](#114-markdown)
	- [1.15 Navigateur web](#115-navigateur-web)
	
2. [Réalisation du projet web](#2-réalisation-du-projet-web)
    - [2.1 Installer l'environnement de développement](#21-installer-lenvironnement-de-développement)
    - [2.2 Démarrer un nouveau projet web](#22-démarrer-un-nouveau-projet-web)
    - [2.3 Prévisualisation de l'application dans le browser](#23-prévisualisation-de-lapplication-dans-le-navigateur-web)
    - [2.4 Utiliser bower pour installer des paquets](#24-utiliser-bower-pour-installer-des-paquets)
    - [2.5 Créer son CV](#25-créer-son-cv)
        * [2.5.1 index.html](#251-indexhtml)  
        * [2.5.2 main.css](#252-maincss)  
        * [2.5.3 main.js](#253-mainjs)  
    - [2.6 Installer GitHub](#26-installer-github)
    - [2.7 Utilisation de Git](#27-utilisation-de-git)
         * [2.7.1 GitHub Pages](#271-github-pages)
         * [2.7.2 Commandes régulièrement utilisées](#272-commandes-régulièrement-utilisées)
    - [2.8 Déploiement](#28-déploiement)
    - [2.9 Tâche gulp git deploy](#29-tâche-gulp-git-deploy)
    - [2.10 Markdown](#210-markdown)
    - [2.11 Release](#211-release)

***

## 1. Présentation des outils
Pour réaliser ce projet web nous allons utiliser différents langages, framework et outils qui seront présentés dans les points suivants.

### 1.1 Éditeur de code
Afin de pouvoir facilement éditer nos codes HTML, CSS et JavaScript il est recommandé d'utiliser un éditeur de code. Un éditeur de code aura l'avantage de nous proposer une colorisation syntaxique. Certains éditeurs de code proposent aussi un système d'autocomplétion, une aide à l'indentation et bien d'autres fonctions nous facilitant l'écriture de code.

Par habitude j'utilise le logiciel Adobe Dreamweaver (CC et CS6). Dreamweaver est un logiciel payant développé par la société Adobe.

Il existe d'autres d'éditeurs de code tel que:

- [Notepad++](https://notepad-plus-plus.org/) _gratuit_

- [Cloud9](https://c9.io/) _gratuit dans une version limitée_

- [WebStorm](https://www.jetbrains.com/webstorm/) _gratuit pour les étudiants_

- [_Plus d'informations sur Adobe Dreamweaver_](http://www.adobe.com/ch_fr/products/dreamweaver.html)
 
### 1.2 HTML
HTML (Hypertext Markup Language) est un language de balisage qui permet de structurer et gérer le contenu texte, image et média d'un site web. HTML est maintenu par le W3C (World Wide Web Consortium). Le W3C édicte également les standards du langage HTML. La version actuelle d'HTML est HTML5 qui a introduit de nouveaux éléments et de nouveaux attributs ainsi que des API.

Dans ce projet nous allons utiliser HTML5 qui est le standard des nouveaux projets web actuel. Nous allons également profiter de l'API `canvas` d'HTML5 pour réaliser un graphique de type "doughnut". 


- [_Plus d'informations sur HTML - W3C_](https://www.w3.org/standards/webdesign/htmlcss)
- [_Plus d'informations sur HTML - MDN_](https://developer.mozilla.org/fr/docs/Web/HTML)


### 1.3 CSS
CSS (Cascading Style Sheets) est un langage qui permet de formater et de faire de la mise en forme des pages web écrites en HTML. Les standards du langage CSS sont aussi définis par le W3C (World Wide Web Consortium).

Dans ce projet nous toucherons peu au CSS, nous allons utiliser le framework Boostrap qui nous met a disposition une très bonne implémentation CSS.

- [_Plus d'informations sur CSS - W3C_](https://www.w3.org/standards/webdesign/htmlcss)
- [_Plus d'informations sur CSS - MDN_](https://developer.mozilla.org/fr/docs/Web/CSS)

### 1.4 JavaScript
JavaScript est un langage de programmation de scripts exécuté par le navigateur Web du visiteur. Le code JavaScript va permettre de dynamiser le contenu d'un site web.

Dans ce projet nous allons utiliser du JavaScript avec la libraire jQuery.

- [_Plus d'informations sur JavaScript - MDN_](https://developer.mozilla.org/fr/docs/Web/JavaScript)

### 1.5 jQuery
jQuery est une librairie JavaScript qui permet d'agir plus simplement sur le code HTML, CSS, JavaScript et AJAX. jQuery offre une syntaxe moins verbeuse et tout une liste de fonctions déjà implémentées et fonctionnelles à utiliser à nos souhaits.
>jQuery Write less, do more.

_Le slogan de jQuery_

Dans ce projet nous allons utiliser jQuery pour modifier la structure même de notre projet web après le chargement de la page. Nous avons également besoin de jQuery pour faire fonctionner correctement le framework Bootstrap.

- [_Plus d'informations sur jQuery_](https://jquery.com/)

### 1.6 Bootstrap
Boostrap est un Framework qui permet de développer des pages web "responsive". Bootstrap livre aussi un design et des fonctions JavaScript directement implémentés dans le framework.

Dans ce projet nous n'allons pas réinventer la roue. Nous allons utiliser les bonnes pratiques et les outils mis à disposition par Bootstrap en profitant de son design "responsive" et sa grille en 12 colonnes.

- [_Plus d'informations sur Bootstrap_](http://getbootstrap.com/)

### 1.7 Modernizr
Modernizr est une bibliothèque JavaScript qui est là pour détecter des fonctionnalités spécifiques de HTML et CSS par navigateurs. Modernizr va permettre par exemple de savoir si le navigateur utilisé supporte certaines spécificités HMTL5, CSS3 ou Javascript et de prévoir une alternative en cas de non support.

Dans ce projet Modernizr est installé par notre outil de création de projet web "webapp" de Yeoman, mais nous n'allons pas nous intéresser plus en profondeur à cette librairie dans ce projet.

- [_Plus d'informations sur Modernizr_](https://modernizr.com/)

### 1.8 Node.js & npm
Node.js est une plateforme qui utilise un moteur JavaScript pour une construction plus rapide d'applications.

NPM est un gestionnaire de paquet JavaScript inclut dans node.js.

Dans ce projet nous allons installer node.js (avec NPM inclut) au début du projet pour ensuite installer d'autres outils avec NPM.

- [_Plus d'informations sur node.js_](https://nodejs.org/en/)
- [_Plus d'informations sur npm_](https://www.npmjs.com/)

### 1.9 Yeoman
Yeoman est un outil qui fonctionne en lignes de commande écrites en Node.js et qui combine un générateur de projet, un gestionnaire de dépendances, l'exécution des tests unitaires, un serveur d'application local et l'optimisation du code pour déploiement.

Dans ce projet nous allons générer notre projet web avec Yeoman.

- [_Plus d'informations sur Yeoman_](http://yeoman.io/)

### 1.10 Bower
Bower est un outil qui va installer et gérer les dépendances des projets web.

Dans ce projet nous allons installer toutes les dépendances de notre projet web avec Bower.

- [_Plus d'informations sur Bower_](https://bower.io/)

### 1.11 Gulp
Gulp est un automatiseur de tâches.

Dans ce projet nous allons utiliser différentes commandes que Gulp propose de base et en ajouter une pour automatiser notre déploiement du site "construit".

- [_Plus d'informations sur Gulp_](http://gulpjs.com/)


### 1.12 Git
Git est un logiciel de gestion de versions décentralisé.

Nous allons utiliser Git tout au long du projet pour garder une historisation de nos modifications et de nos implémentations

- [_Plus d'informations sur Git_](https://git-scm.com/)


### 1.13 GitHub
GitHub est un service web d'hébergement et de gestion de développement de logiciels, utilisant le logiciel de gestion de versions Git.

Dans ce projet nous allons installer le client desktop de GitHub qui intègre le logiciel Git. Nous publierons également nos versions de projet sur Github.

- [_Plus d'informations sur GitHub_](https://github.com/)


### 1.14 Markdown
Markdown est un langage de balisage léger. Ce langage à l'avantage que même s'il n'est pas interprété il est facilement lisible par une personne dans un éditeur de texte standard. Les fichiers markdown ont l'extension `.md`

Dans ce projet nous allons écrire un fichier `Readme.md`. Le fichier `Readme.md` sera directement lu et affiché sur la page de notre projet GitHub

- [_Plus d'informations sur Markdown - GitHub markdown_](https://guides.github.com/features/mastering-markdown/)
- [_Plus d'informations sur Markdown - GitHub Cheatsheet_](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

### 1.15 Navigateur web
Pour afficher les pages web nous allons devoir utiliser un navigateur web. Nous allons également débuguer notre projet web directement avec notre navigateur.

Par habitude j'utilise Mozilla Firefox.

Il existe d'autres naviagteurs tel que:
- [Google Chrome](https://www.google.fr/chrome/browser/desktop/) 

- [Apple Safari](http://www.apple.com/fr/safari/) _Seulement pour OS X_

- [Opera](http://www.opera.com/fr)

- [Microsoft Edge](https://www.microsoft.com/fr-ch/windows/microsoft-edge)

- [_Plus d'informations sur Mozilla Firefox_](https://www.mozilla.org/fr/firefox/new/)


***

## 2. Réalisation du projet web
Processus réalisé sur mon projet web "CV Jonathan Charlet"

### 2.1 Installer l'environnement de développement
On va commencer par installer Node.js et ainsi obtenir également NPM.

Node.js est disponible [ici](https://nodejs.org/)

Une fois Node.js installé on va pouvoir utiliser les commandes NPM dans l'interpréteur de commandes pour installer Yeoman, Bower et Gulp avec la commande suivante:
```
$ npm install -g yo bower gulp-cli
```
L'option `-g` de la commande ci-dessus indique à NPM d'installer `yo`, `bower`  et `gulp-cli` de façon globale et pas seulement localement. Installer ces outils de façon globale nous permettra de les utiliser dans n'importe quel projet indépendamment de notre position.

Maintenant que nous avons installé Yeoaman nous pouvons installer un générateur de projet.

Nous allons utiliser le générateur `generator-webapp` de Yeoman que nous allons installer avec la commande suivante :
```
$ npm install -g generator-webapp
```

### 2.2 Démarrer un nouveau projet web
Maintenant que nous avons installé tous nos outils de développement et le générateur `generator-webapp` nous pouvons passer à la création de notre projet web

Tout d'abord créer un nouveau dossier qui sera notre dossier de projet avec la commande suivante:
```
$ mkdir monCV
```

Il faut se déplacer dans ce dossier
```
$ cd monCV
```

Et lancer la commande Yeoman `webapp` (depuis le dossier `/monCV`)
```
$ yo webapp
```

Yeoman va ensuite nous demander ce qu'on veut déployer dans notre nouveau projet web. Décocher Sass pour avoir que Bootstrap et Modernizr (cocher/décocher avec la `touche espace`) et appuyer sur la `touche enter`

Yeoman nous demande finalement quel style de DSL (domain-specific language) utiliser, BDD (Behavior-driven development) ou TDD (Test-driven development). Dans ce projet nous n'allons pas utiliser de DSL mais Yeoman nous impose d'en choisir un. On va donc en choisir un et appuyer sur la `touche entée`

Lancer pour finir la commande suivante pour installer toutes les dépendances de NPM et Bower
```
$ npm install && bower install
```
### 2.3 Prévisualisation de l'application dans le navigateur web
Pour démarrer le serveur web Gulp il faut lancer la commande suivante :
```
$ gulp serve
```

La commande ci-dessus va ouvrir notre navigateur web avec notre projet web qui se trouve dans le répertoire `/app` .

Maintenant si on modifie notre fichier `app/index.html` et qu'on enregistre, notre navigateur web devrait s'auto rafraichir.

Pour arrêter le serveur web gulp il suffit de faire `CTRL+C` dans l'interpréteur de commandes où l'on a lancé `gulp serve`

### 2.4 Utiliser bower pour installer des paquets
Maintenant que notre projet web est créé et prêt nous pouvons lui ajouter des paquets

Nous allons maintenant installer les paquets que nous utiliserons dans ce projet avec les commandes suivantes :

```
bower install jquery-smooth-scroll --save
```
La commande ci-dessus va installer jquery-smooth-scroll. Ce plugin nous permettra de faire des liens de défilement animé agréable à la place des défilements instantané

```
bower install chartjs --save
```
La commande ci-dessus va installer chartjs. Ce plugin nous permettra de faire des graphiques avec les `canvas` d'HTML5

Avec l'option `--save` toutes les dépendances sont automatiquement enregistré dans bower.json
>When `--save` flag is used, all additional endpoint are saved to dependencies in bower.json.
>Bower recommends to always use --save flag to achieve reproducible installs between machines. 


### 2.5 Créer son CV
Nous allons pouvoir créer notre page web CV en utilisant 3 fichiers de code
* `app/index.html`  Pour notre code HTML5
* `app/styles/main.css` Pour notre code CSS
* `app/scripts/main.js` Pour notre code JavaScript

##### 2.5.1 index.html
Pour la page `app/index.html` je suis parti sur l'exemple Bootstrap "jumbotron" et j'ai ajouté 4 `<div class="row">` dans son contenu.

Dans la zone `div class="jumbotron"` j'ai séparé mon contenu en deux colonnes. `<div class="col-md-3">` pour ma vignette photo et `<div class="col-md-9>"` pour mon adresse personnel.

Dans mes 4 `<div class="row">` je n'ai pas séparé mon contenu en plusieurs colonnes. J'utilise qu'une seule colonne `<div class="col-md-12">` qui contient le contenu texte de mes différentes parties.


##### 2.5.2 main.css
Dans la page `app/styles/main.css` j'ai redéfini la police d'écriture ainsi que la couleur d'écriture pour l'ensemble du texte de ma page.

```CSS
    body{
		font-family:Segoe UI,Tahoma,Verdana,Arial,sans-serif;
        color:#7c7c7c;
    }
```


J'ai changé les couleurs d'écriture de mes titres `h1`,`h2`, `a` et j'ai mis en gras la police d'écriture du contenu texte de ` adress`

```CSS
 h1{
	 color:#4688c8;
	 }
 
 h2{
	color:#4688C8;
	}

a{
	color:#4688C8;
}

address{
	font-weight:bold;
}

```


J'ai aussi agrandi le contenu texte de `id="titre"`
```CSS
#titre{
		font-size:36px;
}
```



##### 2.5.3 main.js
Dans la page de code JavaScript `app/scripts/main.js` j'ai appelé le plugin smoothScroll et j'ai redéfini deux paramètres. La vitesse à 350 millisecondes au lieu de 500 pour être plus rapide et l'offset à -50 au lieu de 0 pour ne pas avoir de décalage quand on retourne tout en haut de ma page.

```JavaScript
  $('a').smoothScroll({offset: -50, speed: 350}); 
```
J'ai aussi ajouté un script qui va rechercher toutes les barres de progressions pour les remplacer par des `<canvas>`. Ces `<canvas>` sont les zones de dessins pour mon plugin Chartjs qui vont afficher un graphique de style "doughnut".

Le code va parcourir le DOM à la recherche de de `<div class="progress-bar>"` et pour chaque `<div class="progress-bar>"` il va récupérer sa valeur et sa couleur depuis ses attributs, il va ensuite remplacer l'élément parent de `<div class="progress-bar>"` qui est `<div class="progress>"` par un `<canvas>`. Une fois ce `<canvas>` créé il va le remplir avec notre graphique "doughnut" correspondant à la barre de progression récupérée avant son remplacement avec ChartJS.


```JavaScript
$('.progress-bar').each( function (){ // Pour chaque <div class=".progress-bar">
    var val= $(this).attr('aria-valuenow'); // on récupère la valeure
    var color = $(this).css('background-color'); // on récupère la couleur
    var newDomElem = $('<canvas ></canvas>'); //création d'un nouvel élément DOM de type canvas
    $(this).parent().replaceWith(newDomElem); // on remplace le parent .progress-bar (.progress) par nos nouveaux canvas
    
        var data = {
            labels: [
                val + '% maitrisé',
            ],
            datasets: [
                {
                    data: [val, 100-val],
                    backgroundColor: [
                        color, '#FFFFFF'
                    ],
        			borderColor: [
                        color, '#FFFFFF'
                    ],
                    hoverBackgroundColor: [
                        color, '#FFFFFF'
                    ],
        			hoverBorderColor: [
                        color, '#FFFFFF'
                    ]
                }]
        };
    
        var myDoughnutChart = new Chart(newDomElem, {
            type: 'doughnut',
            data: data,
        	options: {
        			tooltips:{enabled:false}
        			}
        });
});
```

### 2.6 Installer GitHub
Maintenant que notre projet est prêt nous aimerions suivre son évolution. On va installer GitHub Desktop qui comprend l'outil Git pour faire un suivi de versions et d'évolution de notre web.

GitHub Desktop disponible [ici](https://desktop.github.com/). Une fois le logiciel de bureau GitHub installé nous aurons implicitement Git.

### 2.7 Utilisation de Git
Maintenant que Git est installé, nous allons pouvoir créer notre premier dépôt local de notre projet avec la commande 
```
$ git init
```

On va ajouter un instantané de tous les fichier, en préparation pour le suivi de version
```
$ git add .
```

Et commiter notre première version 
```
$ git  commit -m "Create new project"
```



Nous pouvons maintenant lier ce dépôt Git local `Master` avec le dépôt distant GitHub `Master` en utilisant la commande suivante 
```
$ git remote add origin git@github.com:heg-web/moncv-JoCharlet.git
```

Nous pouvons maintenant envoyer notre dépôt courant  `Master` au dépôt distant `Master`
```
$ git push -u origin master
```
L'option `-u` ajoute une référence de tracking 
>For every branch that is up to date or successfully pushed, add upstream (tracking) reference

##### 2.7.1 GitHub Pages
Github propose d'héberger directement nos sites web avec le service GitHub Pages. 

Nous devons commencer par créer une nouvelle branche sur GitHub qui se nommera `gh-pages` et y envoyer notre projet web construit. Cette branche `gh-pages` doit impérativement avoir à la racine le fichier `index.html`.

L'url du site web sera ensuite http://[username].github.io/[repository] 

[_Plus d'informations sur le service GitHub Pages_](https://pages.github.com/)

##### 2.7.2 Commandes régulièrement utilisées
Un petit extrait des commandes disponible avec Git

Commandes | Explications
------------ | -------------
`$ git init `| Crée un dépôt Git local 
`$  git status `| Liste tous les nouveaux fichiers et les fichiers modifiés à commiter
`$ git add  [fichier]`| Ajoute un instantané du fichier, en préparation pour le suivi de version
`$ git add .`| Ajoute un instantané de tous les fichier, en préparation pour le suivi de version
`$ git commit -m "[message descriptif]"`| Enregistre des instantanés de fichiers de façon permanente dans l'historique des versions
`$ git reset [fichier]` | Enleve le fichier de l'index, mais conserve son contenu
`$ git branch` | Liste toutes les branches locales dans le dépôt Git courant
`$ git branch [nom-de-branche]` | Crée une nouvelle branche
`$ git checkout [nom-de-branche]` | Bascule sur la branche spécifiée et met à jour le répertoire de travail
`$ git merge [nom-de-branche]`| Combine dans la branche courante l'historique de la branche spécifiée
`$ git branch -d [nom-de-branche]`| Supprime la branche spécifiée
`$ git reset [commit]`|Annule tous les commits après `[commit]`, en conservant les  modifications localement
`$ git reset --hard [commit]`| Supprime tout l'historique et les modifications effectuées après le commit spécifié
`$ git diff [premiere-branche] [deuxieme-branche]` | Montre les différences de contenu entre deux branches
`$ git log`| Montre l'historique des versions pour la branche courante
`$ git remote add origin [URL]` | Lier le dépôt courant avec un dépôt distant
`$ git push -u origin [branche]` | Envoie des fichiers commités du dépôt courant à la branche du dépôt distant
`$ git push -f origin [branche]` | Envoie des fichiers commités du dépôt courant à la branche du dépôt distant en forçant l'envoie (suppression des fichiers du dépôt distant au profit des fichiers du dépôt local)
`$ git pull` | Récupère des fichiers du dépôt distant dépôt au dépôt courant
`$ git pull -f`| Récupère des fichiers du dépôt distant dépôt au dépôt courant en forçant la récéption (suppression des fichiers du dépôt courant au profit des fichiers du dépôt distant)
`$ git clone [url]` | Télécharge un projet et tout son historique de version

### 2.8 Déploiement
Nous pouvons maintenant enfin "construire" notre site web avec la commande
```
$ gulp build 
```

Cette commande va construire le rendu "final" de notre projet web dans le dossier `/dist`. Les dépendances sont ajoutées et le code est minifié et optimisé

Pour avoir un aperçu du rendu construit il faut lancer la commande 

```
$ gulp serve:dist
```
Cette commande va ouvrire dans notre navigateur web notre projet construit (qui se trouve dans le dossier `/dist`)


Il nous reste plus qu'à déployer ce projet "construit" sur notre branche `gh-pages` avec les commandes suivantes:

Initialiser notre dépôt Git
```
$ git init
```

Créer et basculer sur la branche `gh-pages`
```
$ git checkout -b gh-pages
```
L'option `-b`
>Specifying -b causes a new branch to be created as if git-branch[1] were called and then checked out. In this case you can use the --track or --no-track options, which will be passed to git branch. As a convenience, --track without -b implies branch creation; see the description of --track below.

On va ajouter un instantané de tous les fichiers, en préparation pour le suivi de version
```
$ git add .
```

On commite 
```
$ git commit -m 'Create new git'
```

Nous pouvons maintenant lier ce dépôt Git local `gh-pages` avec le dépôt distant GitHub `gh-pages` en utilisant la commande suivante 
```
$ git remote add origin git@github.com:heg-web/moncv-JoCharlet.git
```

Nous pouvons maintenant envoyer notre dépôt `gh-pages` courant au dépôt distant `gh-pages` 
``` 
$ git push -u origin gh-pages
```

### 2.9 Tâche gulp git deploy
Afin d'automatiser le déploiement et profiter des possibilités de Gulp nous allons installer `gulp-deploy-git` avec la ligne de commande suivante:

```
npm install --save-dev gulp-deploy-git
```

Il faut ensuite modifier le fichier `gulpfile.js` qui se trouve dans notre projet et y ajouter les lignes suivantes

```JavaScript
var deploy = require('gulp-deploy-git');
gulp.task('deploy', function() {
  return gulp.src('**/*',  { read: false, cwd: 'dist'  })
    .pipe(deploy({
      repository: 'git@github.com:heg-web/moncv-JoCharlet.git',
      remoteBranch:   'gh-pages'
    }))
});
```

Maintenant grâce à `gulp-deploy-git`, nous pourrons déployer un projet "construit" directement sur notre dépôt distant `gh-pages` avec la commande

```
$ gulp deploy 
```


### 2.10 Markdown
Maintenant que notre projet est en ligne sur GitHub nous pouvons lui ajouter un fichier de type Markdown pour présenter notre projet et donner des indications.

GitHub va automatiquement récupérer le fichier nommé `Readme.md` pour l'afficher sur la page principale du projet

Pour créer un fichier `Readme.md` il suffit simplement de cliquer sur le bouton prévu à cet effet sur GitHub et ensuite l'éditer ou alors ajouter un nouveau fichier texte à notre projet et le renommer `Readme.md`. Il ne faut pas oublier de "pusher" ce nouveau document une fois créé et édité 

### 2.11 Release
GitHub gère une notion de "release". Créer une release va créer une version délivrable de notre projet sur GitHub.

Pour créer une nouvelle release il suffit d'aller sur la page de son projet sur GitHub, cliquer sur `releases` et cliquer sur `Create a new release` ou alors si ce n'est pas notre première release `Draft a new release`.

Il faudra pour finir donner un "tage name" à notre release, un titre de release ainsi qu'une description et cocher ou non si c'est un pre-release.

Pour valider la release il faut cliquer sur `Publish release`


***
_Jonathan Charlet_






