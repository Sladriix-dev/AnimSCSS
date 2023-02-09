1.
    il est possible d’animer autant de propriétés que l’on veut avec les transitions ;

    le mot clé   all  permet d’appliquer des transitions simultanément à toutes les propriétés ;

    ou bien on peut séparer les animations par des virgules, ce qui permet de leur donner des valeurs différentes. Exemple :  transition: transform 450ms, background-color 300ms;

    on peut décaler le départ des transitions avec  transition-delay ;

    la valeur de  transition-delay  peut également être définie directement dans la propriété  transition


2.
l’accélération et la décélération des transitions sont contrôlées par la propriété  transition-timing-function ;

si aucune fonction de timing n’est indiquée, la transition utilisera la fonction  ease. Elle suit un profil d’accélération plus net, et une rampe de décélération plus prononcée ;

parmi les autres mots clés pour les fonctions de temporisation, on peut trouver  ease-in,   ease-out,   ease-in-out, et  linear ;

quand aucune fonction de timing par défaut ne correspond à l’animation, il est possible de créer ses propres courbes d’animation personnalisée à l’aide de la fonction  cubic-bezier()  ;

il existe des outils pour ajuster les effets de timing avec la fonction  cubic-bezier()


3.
plus le FPS est élevé, plus l'animation est fluide ;

le taux d’images par seconde idéal est 60 FPS ;

les quatre étapes de la création d’une page web sont : 

    Style : le navigateur comprend la structure HTML du code qu'il reçoit et prépare le style qui sera appliqué,

    Layout (mise en page) : le navigateur détermine la mise en page et la taille des éléments en fonction du style qu'il a reçu,

    Paint : il transforme les éléments en pixels,

    Composition : il combine tous les éléments pour composer la page qui s’affiche ;

pour assurer la fluidité des animations, il faut se contenter d’animer des propriétés de l’étape composition. Les plus utiles sont  transform  et  opacity


4.
la propriété  transform  nous permet de manipuler et animer nos sites de presque toutes les manières, et comme tout se passe pendant l’étape composition, les animations sont bien fluides sur tous les supports ;

on peut déplacer des éléments avec les fonctions translate :   translate(),  translateX(),  translateY()  et  translate3d()  ;

on peut agrandir avec les fonctions scale :  scale(),   scaleX(),  scaleY()  et  scale3d()  ;

et on peut les faire pivoter grâce aux fonctions rotate :  rotate(),  rotateX(),  rotateY() et  rotateZ()  ;

si on ajoute une deuxième propriété  transform, elle annule la première. On ne peut donc définir qu’une seule propriété  transform  dans un même sélecteur ;

pour effectuer plusieurs transformations, on peut les lister dans une même propriété transform comme 
transform:translateX(200%) scale(2)

