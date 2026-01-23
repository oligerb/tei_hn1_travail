
# Chants Québécois

Ce projet d'édition s'inscrit dans le cadre du cours "Éditions de texte : introduction à l'édition numérique avec TEI", donné par Monsieur F. Beretta, à l'Université de Neuchâtel. 

Mon projet vise à transformer en TEI et à annoter un extrait de chansons françaises et canadiennes anciennes sortant du livre "La lyre canadienne : répertoire des meilleureds chansons et romances du jour" de Joseph Lenoir-Rolland sous son pseudonyme "Un amateur", publié en 1847. Pour ce faire, j'ai utiliser les versions numériques trouvées dans "fonds de données linguistiques du Québec".

Le finalité de l'édition (en termes d'éditorialisation) est d'ajouter une annotation sémantique aux textes permettant au public de découvrir plus facilement leur contentu. J'ai pour cela choisi 3 thèmes; L'amour, la nature et la douleur. Grace à la balise `seg` et son attribut `ana`, j'ai pu mettre en avant tout les passages traitant de ses thèmes. J'ai également annoté chaque ligne avec la balise `l` à l'intéreieur du groupe `lg`. 


### Ecodage TEI
Avant de commencer l'encodage, il a fallut faire différents choix. Premièrement, j'ai du choisir la structure générale. Je pensais d'abord partir sur un structure de corpus, regroupant plusieurs chansons indépendantes. Cependant, après réflexion, je me suis rendu compte que une strucutre avec des divisons de groupe suffisait pour mon édition. De cette manière, j'ai un seul "header" pour toutes les chansons, ce qui dans mon cas fonctionne, car elles ont été rassemblées dans un ouvrage par une seule personne. Je n'ai donc pas de métadonnées propre à chaque chant. J'ai donc un seul bloc de métadonnées qui s'appliquent à tout les chants.

Les différents chants sont séparé par `div type="chant"`.Comme déjà mentionné, j'ai décidé d'utiliser les balises suivantes:  `seg`, `l` et `lg`. 


Tout les documents en lien avec l'édition sont entreposer et stocké sur un dépot GitHub. Celui-ci est divisé en différents dossiers. Le dossier final "tei_hn1_travail-1", contient d'une part le sous-dossier "documents_tei" l'édition finale en xml, le css qui permet sa mise en forme ainsi que le schéma xsd qui impose les balises et d'une autre part le sous-dossier "documentation" qui contient l'odd servant à documenter le schéma xsd ainsi qu'un document en markdown qui décrit les requêtes x-path effectuées et finalement le document-ci. 

Pour terminé, j'ai crée un index en html qui fait office de page d'accueil pour mon édition. On y trouve un index des chansons avec ses liens, un index des thèmes et un lien vers l'édition dans son entier.