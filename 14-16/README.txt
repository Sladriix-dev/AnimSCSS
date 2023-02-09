1.
    les animations @keyframes nous permettent de construire des animations plus complexes en créant plusieurs étapes pour les propriétés tout au long de l'animation ;

    les keyframes CSS sont instanciées à l'aide de la règle @keyframes suivie d'un nom pour l'ensemble des keyframes :

        @keyframes example-frames {...} ;

    chaque keyframe peut être établi en utilisant comme valeur le pourcentage d'animation réalisé :

        33% {...} ;

    si vous n'avez besoin que d'un keyframe de début et de fin, les mots clés « from » et « to » peuvent être utilisés à la place de 0 % et 100 % respectivement ;

    si aucun keyframe de début ou de fin n'est fourni, l'animation commence et/ou se termine avec les valeurs de propriété assignées au sélecteur. Si aucune valeur n'est explicitement assignée dans le sélecteur, c'est la valeur par défaut qui est choisie ;

    une animation définie par la règle @keyframes peut contenir différents keyframes avec des propriétés distinctes ;

    plusieurs pourcentages peuvent être assignés à un seul keyframe. Les valeurs définies dans ce keyframe seront appliquées à ces pourcentages dans l'animation ;

    les propriétés et valeurs d'un ensemble de keyframes remplaceront les valeurs de propriétés attribuées à un sélecteur au cours de l'animation.


2.
    les animations CSS @keyframes peuvent être déclenchées en utilisant des pseudoclasses telles que  :hover, tout comme les transitions ;

    les @keyframes CSS peuvent également être déclenchés par le chargement des éléments auxquels ils sont assignés, comme un sélecteur. Par exemple, dès le chargement d'une page ; 

    nous pouvons retarder le démarrage des animations avec keyframes en utilisant la propriété  animation-delay, avec un délai exprimé en secondes ou en millisecondes, tout comme les transitions ;

    nous pouvons étendre ces valeurs du début à la fin de ces animations en utilisant la propriété  animation-fill-mode :

        le mot clé « backwards » prolonge les valeurs de départ d'une animation avant son lancement, couvrant la durée du délai assigné avant que l'animation elle-même ne commence,

        le mot clé « forwards » prolonge les valeurs finales d'une animation jusqu'à ce que la page soit rechargée ou que le navigateur soit fermé,

        le mot clé « both » prolonge l'animation dans les deux sens ;

    nous pouvons définir une fonction de timing des @keyframes en utilisant la fonction animation-timing-function sur le sélecteur où l'animation a été assignée ;

    nous pouvons également définir un timing spécifique keyframe par keyframe, en assignant la propriété  animation-timing-function  aux keyframes en question.


3.
    nous pouvons répéter un ensemble de keyframes autant de fois que nous le souhaitons en utilisant la propriété  animation-iteration-count, avec le nombre de cycles comme valeur ;

    nous pouvons régler nos keyframes pour qu'ils se répètent à l'infini en utilisant la propriété  animation-iteration-count  avec le mot clé « infinite » ;

    la propriété  animation-direction  nous permet de lire un ensemble de keyframes normalement, avec le mot clé « normal » ;

    la propriété  animation-direction  nous permet de lire un ensemble de keyframes vers l'arrière avec le mot clé « reverse » ;

    la propriété  animation-direction  nous permet de lire un ensemble de keyframes avec des allers-retours avec le mot clé « alternate » ;

    et enfin, la propriété  animation-direction  nous permet de lire un ensemble de keyframes avec des allers-retours, mais en commençant par la fin avec le mot clé « alternate-reverse » ;

    nous pouvons mettre en pause une animation avec keyframe en assignant à la propriété  animation-play-state  la valeur réglée sur « paused » ;

    nous pouvons reprendre la lecture d'une animation avec keyframe en assignant la propriété  animation-play-state  avec la valeur réglée sur « running ».