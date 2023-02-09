1.
    transform-origin  permet de repositionner le point d’ancrage, qui se trouve par défaut au centre de l’élément ;

    on peut régler ce point d’origine en utilisant des unités comme px, rem, vh, etc. ;

    il est aussi possible d'utiliser des pourcentages pour X et Y ;

    ou encore, on peut utiliser des mots clés :  left  et   right  pour l’axe X,  top  et  bottom  pour l’axe Y, et  center  pour les deux ;

    il est possible de ne pas indiquer la valeur de l'axe Y ou, quand on utilise des mots clés, de mettre uniquement une valeur : le navigateur comprend de lui-même à quel axe la valeur s'applique ;

    quand on change le point d’origine en 3D, la valeur de Z doit être exprimée en unités (et non en pourcentages) ! 



2.
    animer la couleur d’une propriété déclenche des calculs de paint ;

    la propriété  opacity  nous permet de faire des transitions entre des couleurs en évitant ces calculs ;

    la propriété  opacity  reçoit une valeur entre 0 et 1, 0 étant complètement transparent et 1 complètement opaque ;

    pour éviter d’avoir à ajouter des  <div>  supplémentaires, que l'on aurait dû ajouter à chaque fois dans le HTML, on peut utiliser le pseudoélément  ::before  ou  ::after  ;

    pour créer un pseudoélément, ajoutez le nom du pseudoélément à un sélecteur, en utilisant le préfixe double deux-points :  .selector::after{...}

    les pseudo-éléments   ::before  et  ::after  créent un élément qui est respectivement le premier ou le dernier enfant de l’élément sélectionné ; 

    il est possible de créer des dégradés de couleur. Il suffit d'attribuer un dégradé au background-color de l'élément d'arrière-plan. On fera ensuite disparaître l'élément superposé avec opacity: 0.


3.
