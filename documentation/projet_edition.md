
# Chants Québécois

Ce projet d'édition s'inscrit dans le cadre du cours "Éditions de texte : introduction à l'édition numérique avec TEI", donné par Monsieur F. Beretta, à l'Université de Neuchâtel. 

Mon projet vise à transformer en TEI et à annoter un extrait de chansons françaises et canadiennes anciennes sortant du livre "La lyre canadienne : répertoire des meilleureds chansons et romances du jour" de Joseph Lenoir-Rolland sous son pseudonyme "Un amateur", publié en 1847. Pour ce faire, j'ai utiliser les versions numériques trouvées dans "fonds de données linguistiques du Québec".

Le finalité de l'édition (en termes d'éditorialisation) est d'ajouter une annotation sémantique aux textes permettant au public de découvrir plus facilement leur contentu. J'ai pour cela choisi 3 thèmes; L'amour, la nature et la douleur. Grace à la balise ```` seg ana```` j'ai pu mettre en avant tout les passages traitant de ses thèmes. J'ai également annoté chaque ligne avec la balise ```l``` à l'intéreieur du groupe ````lg````. 


### Ecodage TEI
Avant de commencer l'encodage, il a fallut faire différents choix. Premièrement, j'ai du choisir la structure générale. Je pensais d'abord partir sur un structure de corpus, regroupant plusieurs chansons indépendantes. Cependant, après réflexion, je me suis rendu compte que une strucutre avec des divisons de groupe suffisait pour mon édition. De cette manière, j'ai un seul "header" pour toutes les chansons, ce qui dans mon cas fonctionne, car elles ont été rassemblées dans un ouvrage par une seule personne. Je n'ai donc pas de métadonnées propre à chaque chant. 

Comme déjà mentionné, j'ai décidé d'utiliser les balises  ```` seg ana```` , ```l``` et ```lg```. 

Ensuite, j'ai choisi 