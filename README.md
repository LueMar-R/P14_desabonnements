# P14_desabonnements

Ludivine

<hr>



On cherche à prédire le désabonnement des clients : ils s'agit d'un problème de
__classification binaire__, car on cherche à savoir si oui (1), le client va se désabonner, ou bien si non (0), le client va rester.</p>

Nous allons utiliser un modèle de perceptron multicouche pour résoudre ce problème de classification. Les paramètres à utiliser sont les suivants :

- La dimension de la couche d'entrée doit correspondre au nombre de caractéritiques d'entrée (= nombre des features = taille de X), càd __13 neurones__.
- La dimension de la couche de sortie sera de 1 neurone, puisqu'on a une seule classe de sortie, la probabilité de désabonnement. On utilisera une __fonction sigmoïde__ en sortie pour estimer cette probabilité, et __l'entropie croisée binaire__ pour la fonction de perte.
- pour les couches cachées, nous utiliserons la fonction d'activation ReLu, qui est efficace dans la plupart des cas.

Restent à fixer :

- le nombre de couches cachées et le nombre de neurones qu'elles contiendront,
- l'optimiseur,
- le taux d'apprentissage,
- la taille des lot à l'entraînement,
- le nombre d'epochs.

Différents parametres seront testés dans ce notebook. Les résultats obtenus tournent autour de 86% de prévisions correctes.
