# Partie I <head>
 ## Balise html lang="Default"
    --> remplacé par langue="fr".


 ## Dans la balise "meta keywords", le contenu ne correspond pas parfaitement au contenu du site et il y a bcp de répétition, en plus, c'est une agence à Lyon, pas à Paris. il faut préciser et varier les mots-clés plus pertinents.
    --> remplacé par exemple par "seo, site web, agence de webdesign à Lyon, agence design, création du site".


## Il manque la description dans la balise "meta description"
    --> On peut ajouter "L'agence le Cerf est l'une des meilleurs agence de webdesign à Lyon, qui vise à aider les entreprise à devenir attractives sur Internet". 

## Il faut ajouter le link 'bootstrap.min.css' pour minimiser la taille de fichier.

## Il faut mettre les JS en bas du body et enlever le "defer"

## Il manque un titre
    --> Agence le Cerf-Une des meilleures agences de Webdesign à Lyon.

# Partie II 
## les balise ne sont pas sémantiques, au lieu d'utiliser "header, section, main et footer" etc., j'ai vu que le ".container" va du haut jusqu'au bas, pour le robot d'indexation, il confuse pour attraper les info pertinentes.
    --> donc j'ai ajouté les balises comme <header> <main> <section> et <footer> dans l'emsemble du site.

## 2.1 Bloc-0 
 Dans la partie <header>
 ### J'ai barré la partie ".navbar-header", car c'est black hat".

 ### Dans la partie ".navbar-header", pour l'image de logo, il faut corriger la localisation d'agence dans "alt" pour optimiser la capturtation correcte des info.
 --> alt="logo de l'agence le cerf- meilleure agence webdesign à Lyon".

 ###  Dans le <div class="collapse navbar-collapse navbar-1 special-dropdown-nav">, le deuxième item de navigation n'est pas clair, donc:
     -->Remplacer "page 2" par "Contactez-nous" par exemple.

 ### Toujours dans cette partie, la navigation ne peut pas bien résumer les section de la page, donc c'est mieux de compléter les items dans la navigation pour bien montrer aux visiteurs les keywords (contenu principal) de la page et augmenter les fréquences des apparitions des keywords.
     --> Par exemple, j'ai ajouté 'nos services, nos objectifs, nos réalisations' selon le contenu de cette page.

### Après avoir ajouté les items dans nav, il liste dans un colonne, donc dans le style.css, j'ai ajouté dans la ligne '332': 
     --> .navbar-nav{
    flex-direction: row;
}
et dans la ligne 9: a{
    text-decoration: none;
}


 ## 2.2 Bloc-1-présenttion

  ### Le même problème sur alt, c'est à Lyon, il faut pas donner les fausse infos pour le robot d'indexation. Donc je renomme le nom de l'image logo (logo-agence du Cerf.png) pour optimiser SEO.
 --> alt="Agence le Cerf, agence web Lyon, création logo Lyon".
     Je corrige la taille de logo pour être plus visible pour les visiteurs

   ### Dans le <h1> je corrige la couleur en blanc, car la couleur en #896cf3 n'est pas lisible.

## 2.3 Bloc-2-Service 
### Dans cette partie, je remplace l'image par le texte en donnant un attribut, car le robot d'indexation ne reconnait pas le contenu de l'image. 
--> <h2 class="fs-1">L'agence le Cerf est une agence de webdesign qui aide les entreprises à devenir attractives sur Internet</h2>

### J'ai supprimé le '&rsquo' dans le preimer text et le '&nbsp;', '<br> dans le deuxième, car je pense que ce n'est pas très utile.

### Je change les balises <span> par les balises <i>, car ce sont les icons, si on utilise <i> c'est plus cohérent. 

### Je corrige le taille police <p> de 11px à 14px pour plus lisible.

### Dans le div .med-width-whitespace, je supprime dans le css {box-shadow: 0px 0px 0px #000000;}; et je change le max-width: 1200px pour qu'il y ait plus d'espace entre les trois bloc services.

### Pour la citation de Maxime Guibard, il faut aussi le changer en texte, la même raison comme ci-dessus, et j'ai ajouté <strong> pour la phrase"L'agence du Cerf est l'une des meilleures de Lyon".
    --> <figure class="col-xs-12 col-md-8 col-md-offset-2 text-center">
            <blockquote class="blockquote">
                <p class="fs-2">
                    "<strong>L'agence du Cerf est l'une des meilleures de Lyon</strong>, grâce à elle, nous avons pu doubler notre visibilité en ligne et notre chiffre d'affaires a bondi. J'hésiterais pas une seule seconde à recommander l'agence du Cerf"
                </p>
            </blockquote>
            <figcaption class="blockquote-footer fs-2">
                Maxime Guibard, PDG de A vos tourchettes
            </figcaption>
        </figure>

## 2.4 Bloc-3-What-I-do
### Je change le titre <h2> en couleur blanche et la taille de police du texte pour la rasion de lisibilité. Comme dans le style.css a déjà nommé ltc-text:white; donc juste corrigé tc-white en ltc-white:
    --> class="ltc-white";
        class="fs-4"

### J'ai supprimé les balises <br> à la fin du titre et duu texte et changé la place de link <a> dehors du balise <p>, et dans le style.css, je change comme ci-dessous:
    --> .bold-link {
     margin-left:150px;
    /* text-decoration: underline!important; */
         }

## 2.5 Bloc-4-portfolio
### Pareil, changer la photo par le titre <h2>:
    --><h2 class="fw-bolder">Nous travaillons avec beaucoup de clients, voici nos réalisations.</h2>

### Pour les titres de chaque portfolio, j'ajoute la balise <strong> sur les premiers mots qui liée l'oblectif et la description du site, par exemple:
    --> <h3 class="mg-md text-center">
           <strong>Création d'un site internet</strong> pour un voyageur
        </h3> 

## 2.6 Bloc-5-cta
### J'ai ajouté un attribut pour <h2> pour la raison de visibilité:
    --> <h2 class="mg-md text-center ltc-white display-4">
		   Prêt pour redonner vie à votre projet ?<br>Contactez notre équipe !
		</h2>
### J'ai suppimé la classe="bloc-bg-texture", sinon, on ne peut pas sélectionner le titre.

# Partie III
## Changer le <p> par <h4> et supprimer <br>
    --><h4 class="text-center white">
		  Agence le Cerf - Agence web basée à Lyon.
	   </h4>

## Changer toutes les balises <span> par <i> pour les icons social.

## Supprimer les lien dans icons, car selon l'évaluation de Wave, il s'agit des liens redondants.

## Supprimer le div .keyword, piage, black hat.

## J'ai supprimé  h4 {color: #333333!important;}dans le style.css, ligne 739 pour h4, sinon, c'est pas visible. Et ajouter class="class="ltc-white"
    --><h4 class="ltc-white">Partenaires</h4>

## Dans style.css, ligne 23, j'ai ajouté:
    --> li{
    list-style-type: none;
           }
## Dans les balises <li>><a>, j'ai ajouté lass="class="ltc-white", j'ai essayé de le mettre dans le parent de <li>, mais cela ne fonctionne pas...

## J'ai donné un class .partenaires dans le <ul> pour la mise en place des partenaires, dans le style.css, ligne 375:
    -->footer .partenaires li{
    margin-bottom: 10px;
    font-size: 18px;    
        }

## Pour les liens dans le "partenaires", ce sont des liens invalides, donc je les ai remplacés par les liens valides en réécrivant les noms de partenaires correspondants. 

## J'ai supprimé les deux annuaires identiques en ajoutant deux autres blocs qui sont pertinents pour ce site. (je ne comprends pas trop qu'est-ce que ça veut dire 'annuaire list'...)

 


# Page 2.html

# Partie I <head>

## Comme l'index.html, balise html lang="Default"
    --> Remplacé par langue="fr".

## Il faut ajouter les mots-clés dans la balise "meta keywords":
    --> "seo, site web, agence de webdesign à Lyon, agence design, création du site".


## Il manque la description dans la balise "meta description"
    --> On peut ajouter "Vous souhaitez en savoir plus sur nos services et les propositions sur vos projets de webdesign? N'hésitez pas à nous contactez par email ou par téléphone". 

## Il faut mettre les JS en bas du body.

## Il faut ajouter le link 'bootstrap.min.css' pour minimiser la taille de fichier.

## Il manque un titre
    --> Contacter notre Agence le Cerf pour vos projets

# Partie II <body>
## bloc-0
### Changer la nav identique comme dans le page d'accueil.


## bloc-6
### Remplacer ".tc-white" par ".ltc-white"

## bloc-7
### Dans chaque <label>, ajouter for="" pour préciser.
### J'ai ajouté class="display-6 text-dark" dans chaque label pour être visible.
### Pour label <label for="prjet webdesign" > il y une erreur orthographe 
    -->projet

### Supprimé <br> derrière "Brief de votre projet (Ajoutez autant de détails que nécessaire)"


# Partie III <footer>

## bloc-8
### Remplacer <div> par <footer>

### Changer le <p> par <h4> en ajouer <strong> pour le mot-clé "Agence web basée à Lyon":
    --><h4 class="text-center white">
		   Agence Le Cerf - <strong> Agence web basée à Lyon</strong>.
	   </h4>

### Changer le <span> par <i> pour les icons.

### J'ai déplacé le bloc sur le contact dans le <footer>, car je pense que c'est plus logique. Et j'ai reformulé le contenu:
    --> <div class="col-sm-6">
            <h4 class="ltc-white"> Nous contactez</h4>
            <p>Agence le Cerf - Web design</p>
            <p>contact@agencelecerf.com	</p>
            <p>2 place Sathonay, 69001 Lyon</p>
            <p>Ouvert de 9h à 18h, du lundi au vendredi</p>
            <p>Web:<a href="index.html">CerfLYon-Design</a> </p>
			
		</div>