Title: Utiliser les liens
Slug: tutorial-links
Lang: fr
Author: stimbale
Translation: true

Ce tutoriel explique comment ajouter des hyperliens dans les documents Sozi et comment lier à un cadre Sozi.

Téléchargez et ouvrez l'exemple de document
-------------------------------------------

Ce tutoriel est basé sur un document SVG qui contient les éléments visuels de notre présentation.
[Télécharger le document SVG de base] (|filename| /images/tutorial-links/sozi-links-tutorial-base.svg)
(cliquez avec le bouton droit sur le lien et choisissez *Enregistrer la cible du lien sous*) et ouvrez-le dans Inkscape.

![Ouvrir le document SVG de base dans Inkscape] (|filename|/images/tutorial-links/sozi-links-tutorial-screenshot-01.png)

Créer les vues basées sur les cadres
------------------------------------

Sélectionnez les cinq rectangles et ouvrez Sozi dans le menu *Extensions*.
Cadrer chaque vues de la présentation sur les rectangles du documant graphique SVG.
Pour vous aider à identifier facilement chaque rectangle, nous avons déjà défini leurs identifiants pour qu'ils correspondent à leurs couleurs (par exemple l'Id du rectangle *blue* est `blue-rect`).

![Créer un cadre pour chaque rectangle] (| filename |/images/tutorial-links/sozi-links-tutorial-screenshot-02.png)

A la suite, créez cinq cadres avec les propriétés suivantes:

<table>
    <tr>
        <th>Titre</th>
        <th>Id</th>
        <th>Elément SVG</th>
    </tr>
    <tr>
        <td>Black</td>
        <td>black-frame</td>
        <td>black-rect</td>
    </tr>
    <tr>
        <td>Red</td>
        <td>red-frame</td>
        <td>red-rect</td>
    </tr>
    <tr>
        <td>Green</td>
        <td>green-frame</td>
        <td>green-rect</td>
    </tr>
    <tr>
        <td>Magenta</td>
        <td>magenta-frame</td>
        <td>magenta-rect</td>
    </tr>
    <tr>
        <td>Blue</td>
        <td>blue-frame</td>
        <td>blue-rect</td>
    </tr>
</table>

Fermez Sozi et sauvegardez le document.
Vous pouvez déjà l'ouvrir dans un navigateur Web pour vérifier que toutes les images sont correctement définies.

URL d'image
-----------

Lorsqu'un document Sozi est ouvert dans le navigateur Web, le contenu de la barre d'adresse change lorsque vous passez d'une image à l'autre.

![URL de l'image dans la barre d'adresse d'un navigateur Web] (|filename|/images/tutorial-links/sozi-links-tutorial-screenshot-03.png)

Dans l'exemple ci-dessus, la barre d'adresse affiche l'URL:

    file: //.../sozi-links-tutorial-full.svg#green-frame

Si votre document est publié sur un serveur Web, le premier élément sera `http` ou` https` au lieu de `file`.
Les derniers éléments de l'URL sont le nom du fichier SVG suivi d'un caractère *hashtag* (`#`) et l'identifiant de l'image actuelle ("green-frame").

Par conséquent, si vous partagez une présentation sur le Web, il sera possible de faire un lien direct vers n'importe quelle trame avec un Id donné.

Création de liens hypertexte dans une présentation Sozi
-------------------------------------------------------

De retour dans Inkscape, faites un clic droit sur le cercle rouge et choisissez *Créer un lien*.
Cette action n'ouvre aucune boîte de dialogue. Il enveloppe simplement l'élément sélectionné dans un élément de lien SVG.

![Création d'un lien dans Inkscape](|fichier|/images/tutorial-links/sozi-links-tutorial-screenshot-04.png)

Maintenant faites un clic droit sur le cercle rouge et choisissez *Propriétés du lien*.

![Modifier un lien dans Inkscape](|fichier|/images/tutorial-links/sozi-links-tutorial-screenshot-05.png)

La boîte de dialogue suivante permet d'éditer plusieurs attributs du lien sélectionné. Pour créer un lien vers le cadre inclus dans le rectangle rouge, il suffit de définir l'attribut `Href` `# red-frame`. Vous pouvez procéder de même pour les trois autres cercles.

![Définition de l'attribut href d'un lien](|filename|/images/tutorial-links/sozi-links-tutorial-screenshot-06.png)

Lire la présentation dans un navigateur Web
-------------------------------------------

Enregistrez le document dans Inkscape.

Ouvrez le document SVG avec votre navigateur Web préféré.
Il se concentrera automatiquement sur la première image.
Cliquez à l'intérieur du fond blanc du document pour passer à l'image suivante

![Télécharger ou lire la présentation complète](|filename|/images/tutorial-links/sozi-links-tutorial-full.svg).
