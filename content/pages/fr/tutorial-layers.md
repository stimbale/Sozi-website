Title: Utiliser les calques
Slug: tutorial-layers
Lang: fr
Author: stimbale
Translation: true



Une présentation Sozi peut être organisée en un ou plusieurs calques qui se déplacent indépendamment.
Une utilisation typique des calques consiste à ajouter un arrière-plan fixe à vos images.
Mais il existe de nombreuses autres possibilités.
Avec un peu de travail et d'ingéniosité, vous pouvez faire des animations sophistiquées.
Toutefois, rappelez-vous que le but principal de Sozi est de faire des présentations, il ne fournira pas les fonctionnalités que vous attendez d'un logiciel d’animation généraliste.

Téléchargez et ouvrez le document de base
-----------------------------------------

Ce tutoriel est basé sur un document SVG qui contient tous les éléments de dessin de notre présentation.
[Téléchargez le document SVG de base](https://github.com/senshu/Sozi/raw/master/samples/tutorial-layers.svg)
(cliquez sur le lien avec le bouton droit de la souris et choisissez *Enregistrer le lien sous*).

Ce document SVG a été créé avec [Inkscape](https://inkscape.org).
Nous vous recommandons d'installer Inkscape avant de continuer.
Avant de commencer la création de la présentation, nous verrons l'organisation des graphismes.

Ouvrez le fichier 'tutorial-layers.svg' dans Inkscape.

![Le document dans Inkscape](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-01.png)

Organisation des calques
------------------------

Inkscape permet d'organiser un document en calques.
Vous pouvez ouvrir le panneau Calques en cliquant sur le bouton *Calques* de la barre d'outils ou en choisissant *Calques* ... dans le menu *Calque* ou par le raccourci clavier (Maj + Ctrl + L).
 
Dans cet exemple, le document contient trois calques:

* *Caption _(Texte)_*:le calque de premier plan avec des éléments de texte.
* *Landscape _(Paysage)_* : le calque intermédiaire contient le dessin d'un arbre.
* *Sky _(Ciel)_* : le calque d'arrière plan contient un grand cercle bleu avec le soleil, la lune et les étoiles.

Chaque calque a un sous-calque nommée « Frames ». Ces sous-calques contiennent des rectangles qui aideront à aligner les graphiques lors de la création de la présentation Sozi.

>Vous pouvez afficher ou masquer un calque en cliquant sur l'icône "œil" correspondante dans la boîte de dialogue Calques.
>Essayez d'afficher et de masquer chaque calque et sous-calque pour identifier les éléments appartenant à chaque calque.
>
>Assurez-vous que tous les calques sont visibles avant de passer à la section suivante.

Créer les cadres de la présentation Sozi
----------------------------------------

Ouvrez le fichier « tutorial-layers.svg » dans l'éditeur de présentation Sozi.

![Document de base dans Sozi](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-03.png)

Créez quatre images à l'aide du bouton « + » dans le volet de Montage.
Pour chaque image, remplissez le champ Titre avec les titres suivants:

1.	"Matin",
2.	"Midi",
3.	"Soir",
4.	"Nuit".

La timeline ou ligne de temps devrait ressembler à ceci:

![Timeline avec les 4 calques](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-04.png)
 
Ajouter un calque fixe (Paysage)
--------------------------------

Appuyez sur le bouton *Ajouter un calque* et choisissez *Landscape*.
Dans la timeline, sélectionnez la cellule correspondant à la première image et au calque *Landscape* comme indiqué ci-dessous.

![Sélectionner le calque Landscape en calque for frame 1](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-05.png)

Dans la zone d'aperçu, effectuez un zoom avant (molette de la souris) et déplacez le calque *Landscape* jusqu'à ce que le rectangle contenant l'arbre remplisse presque toute la zone.
Assurez-vous que seuls les éléments du calque *Landscape* sont affectés.

![Zoom sur le calque Landcape](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-06.png)

Dans le volet des propriétés à droite, le champ *Id de l'élément à utiliser comme contour* doit indiquer "rect-paysage".
C'est l'identifiant SVG du grand rectangle rouge qui entoure le dessin de l'arbre.
Puisque le bouton de *sélection de l'élément automatiquement* est actif, Sozi propose automatiquement ce rectangle à utiliser comme contour pour le calque en cours.

* Appuyez sur le bouton *Ajuster à l'élément* sur la droite: maintenant le calque *Landscape* a été ajusté de sorte que le rectangle remplisse toute la zone d'aperçu.
* Appuyez sur le bouton *Cacher l'élément* pour masquer le rectangle.

![Sélection de l'élément de contour](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-07.png)

Si la présentation est lue dans une fenêtre de navigateur Web avec des proportions différentes, nous souhaitons masquer les graphiques en dehors de la zone actuellement visible.
Pour cela, en haut à droite du volet des propriétés, appuyez sur le bouton *Clip*.

Nous avons mis en place une calque qui ne bougera pas pendant la présentation.
Maintenant, laissez-nous créer un calque dynamique.

![Ajustement du calque Landscape](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-08.png)

Ajouter un calque dynamique (textes de légendes)
------------------------------------------------

Appuyez sur le bouton *Ajouter un calque* et choisissez *Captions*. Dans la timeline, sélectionnez la cellule correspondant à la première image et au calque *Captions* comme indiqué ci-dessous.


![Sélection du calque des texte en calque 1](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-09.png)

Dans la zone d'aperçu, effectuez un zoom avant (molette de la souris) et déplacez le calque *Captions* jusqu'à ce que le rectangle contenant le texte "Matin" remplisse presque toute la zone.
Assurez-vous que seuls les éléments du calque *Captions* sont affectés.

![Zoom sur le calque des textes](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-10.png)

Le champ *Id de l'élément à utiliser comme contour* devrait indiquer "rect-text-morning".
Appuyez sur les boutons *Ajuster à l'élément*, *Cacher l'élément* et le bouton "Clip".

Appliquer le même processus aux cadres "Midi", "Soir" et "Nuit".
La zone d'aperçu pour chaque image doit ressembler à ceci:

![Ajustement du calque 1 pour le texte](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-11.png)
![Ajustement du calque 2 pour le texte](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-12.png)
![Ajustement du calque 3 pour le texte](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-13.png)
![Ajustement du calque 4 pour le texte](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-14.png)

Ajouter un calque dynamique (Sky)
---------------------------------

À ce stade, tous les graphiques n'appartenant ni au calque *Landscape* ni aux calques *Captions* sont représentés par la ligne *Default* de la timeline.
En général *Default n'est pas réellement un calque: il regroupe tous les calques qui n'ont pas été ajoutés à la timeline et tous les éléments n'appartenant pas à un calque (attention, il faut l'éviter, mais cela peut arriver).
Si vous ajoutez un nouveau calque au document SVG dans Inkscape, il arrivera automatiquement dans la catégorie *Default* de Sozi.

Appuyez sur le bouton *Ajouter un calque* et choisissez *Sky*.
La ligne *Default* devrait disparaître.

Pour plus de commodité, nous allons masquer les calques *Landscape* et *Captions*.
Cliquez sur les icônes "oeil" à gauche dans les lignes correspondant à ces calques.

![Sélectionnez les deux calques](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-15.png)

> L'icône "oeil" permet de masquer un calque dans l'éditeur pendant que vous travaillez sur d'autres calques.
> Les calques masqués sont toujours visibles lors de la lecture de la présentation.
>
> Si vous souhaitez masquer un calque lors de la lecture de la présentation, positionnez la propriété d'opacité du calque à zéro.

Procédez comme vous l'avez fait pour le calque *Captions*.
Pour chaque image:

1. Dans la ligne *Sky* de la timeline, sélectionnez la cellule correspondant à l'image que vous souhaitez modifier.
2. Dans la zone d'aperçu, effectuez un zoom (molette de la souris), déplacez et faites pivoter (Maj + molette de la souris) la couche jusqu'à ce que le rectangle souhaité remplisse presque entièrement la zone.
3. Cochez la case *ID de l'élément*, puis appuyez sur les boutons *Ajuster à l'élément*, *Cacher l'élément* et le bouton "Clip".

Affichez à nouveau les autres calques. La zone d'aperçu devrait ressembler à ceci:

![Ajustement du calque 1 du calque Sky](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-16.png)
![Ajustement du calque 2 du calque Sky](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-17.png)
![Ajustement du calque 3 du calque Sky](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-18.png)
![Ajustement du calque 4 du calque Sky](|filename|/images/tutorial-layers/sozi-layers-tutorial-screenshot-19.png)

Enregistrer et lire la présentation
-----------------------------------

L'éditeur doit enregistrer votre présentation automatiquement.
Si ce n'est pas le cas, vous pouvez suavegarder votre présentation en appuyant sur le bouton *Sauvegarder* dans la barre d'outils.

Ouvrez le fichier tutorial-layers.sozi.html dans un navigateur Web.
La vue est automatiquement positionnée sur la première image de la présentation.
Cliquez dans la fenêtre du navigateur pour passer à l'image suivante. (voir aussi: [Play](|filename|play.md)).

[Téléchargez la présentation complète](https://github.com/senshu/Sozi/raw/master/samples/tutorial-layers.sozi.html)
(cliquez sur le lien avec le bouton droit de la souris et choisissez *Enregistrer le lien sous*).
