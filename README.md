# EXO_TRI

Dans ce checkpoint l'on nous demande de faire le tri par insertion des elements d'un tableau ou une liste

Pour resoudre nous allons diviser le tableau en une partie triée et une partie non triée.

donc nous allons utiliser un compteur i pour parcourir la partie non triée.  
la partie triée pour exister doit contenir au moins un élément qui sera utiliser comme premier élément de comparaison  ce qui implique que le compteur pour parcourir la partie non triée commencera à partir du second élément donc de l'indice 1
nous recuperons l'élément à l'indice i que nous mettons dans une variable tampon.

Nous parcourons la partie  triée avec le compteur j qui est initialisé à la valeur de i
nous parcours en comparant la valeur de la variable tampon à l'élément à l'indice j-1 tant que la variable tampon est inférieur à l'élément indice j-1 c'est à dire à chaque fois  que la condition est vraie  alors nous décalons l'élément d'indice j-1 à l'indice j puis nous faisons une décrementation du compteur ce qui revient à parcourir les élément avec un compteur décroissant. nous repetons cette action jusqu'a ce que la condition n'est plus vraie c'est à dire tampon >= element indicej-1   oubien si le compteur J n'est plus superieur à 0 car l'element à l'indice 0 a permis de faire la dernière comparaison donc impossible de faire une comparaison après donc la boucle s'arrete
alors nous affectons le contenu de tampon au dernier espace qui a été laissé par le décallage

Nous incrementons donc le compteur i pour passer à l'element suivant de la partie non triée et nous repetons laction de comparaison et de decalage jusqu'au dernier element et notre tableau est donc trié et rangé

NB. nous avons utilisé la condition j >0 dans la boucle While car nous avons commencé à parcourir la partie non trié à partir du second élément donc indice 1. si nous avions dabord trié les 2 premiers éléments avant de commencer a parcourir  nous aurions commencé à l'indice 2 dans ce cas cette condition allait nous conduire à  un dépassement d'indice de tableau mais en commençant  directement à l'indice 1 sans faire de premier trie en fixant l'indice 0 on peut pose cette condition pour etre sur que nous somme arrivé en bout de tableau



