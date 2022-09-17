# Algorithme de Gale-Shapley randomisé
Un problème récurrent aux Mines est l'allocation équitable d'objets. Le problème de base est l'allocation d'objets différents, à des agents qui les classent différemment. C'est un sujet de recherche mathématique, avec des papiers proposant diverses solutions algorithmique. Devant la flemme d'implémenter un tel algorithme, non prévu pour le grand public, j'utiliserai un autre algorithme adapté au problème des mariages stables, l'algorithme $Gale-Shapley$. Mais celui s'appuie sur un classement établi par les deux parties du problème (les élèves et les projets).

Le classement des projets pour les élèves sera établi de manière aléatoire. Les élèves proposent et les projets disposent. Cette situation permet d'obtenir la meilleure satisfaction des élèves (et la pire pour les projets mais tant mieux). L'algorithme va tourner plusieurs fois, afin de générer plusieurs configurations, et choisir la plus optimale. Le critère d'optimalité sera le rang du choix obtenu par l'élève le moins bien servi (et le décompte des insatisfaits).  