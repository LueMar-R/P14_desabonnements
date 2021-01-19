# P14_desabonnements

Ludivine

<hr>



<p style="color:#468";>On cherche à prédire le désabonnement des clients : ils s'agit d'un problème de
<span style="font-weight: bold";>classification binaire</span>, car on cherche à savoir si oui (1), le client va se désabonner, ou bien si non (0), le client va rester.</p>

<p style="color:#468";>Nous allons utiliser un modèle de perceptron multicouche pour résoudre ce problème de classification. Les paramètres à utiliser sont les suivants :</p>

    <p style="color:#468";>La dimension de la couche d'entrée doit correspondre au nombre de caractéritiques d'entrée (= nombre des features = taille de X), càd <span style="font-weight: bold";>13 neurones</span>.</p>
    <p style="color:#468";>La dimension de la couche de sortie sera de 1 neurone, puisqu'on a une seule classe de sortie, la probabilité de désabonnement. On utilisera une <span style="font-weight: bold";>fonction sigmoïde</span> en sortie pour estimer cette probabilité, et <span style="font-weight: bold";>l'entropie croisée binaire</span> pour la fonction de perte.</p>
    <p style="color:#468";>pour les couches cachées, nous utiliserons la fonction d'activation ReLu, qui est efficace dans la plupart des cas.</p>

<p style="color:#468";>Restent à fixer :</p>

    <p style="color:#468";>le nombre de couches cachées et le nombre de neurones qu'elles contiendront,</p>
    <p style="color:#468";>l'optimiseur,</p>
    <p style="color:#468";>le taux d'apprentissage.</p>
    <p style="color:#468";>la taille des lot à l'entraînement</p>
    <p style="color:#468";>le nombre d'epochs</p>

<p style="color:#468";>Différents parametres seront testés dans ce notebook. Les résultats obtenus tournent autour de 86% de prévisions correctes.
