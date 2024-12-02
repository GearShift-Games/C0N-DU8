# Paragraphe de présentation


CON D83 (conduite) est un jeu de course interactif intense plein de rebondissements et légèrement humoristique dans lequel l'utilisateur contrôle son véhicule à l'aide d'un vélo stationnaire.

# MVP (Minimal Viable Product)

## Visuel

- Un modèle de véhicule simple
- Un circuit de course simple
- Un UI simple

## Audio

- Musique d'ambiance
- bruits de véhicule

## Interactivité

- Mouvements détectés par senseurs
- Frein fonctionel
- Fin de la course

## Matériel

- 1 Projecteur
- 1 Vélo Stationnaire
- 2 Hauts Parleurs
- 1 capteur opencv blob tracking centroid
- 1 Écran Tactile
- 2 Bouton
 


# [Lien GitHub](https://github.com/GearShift-Games/CON-D83/tree/main)

# Date de livraison des test :

## 28 Février 2025

# Risques:

- R1: Détection des mouvements de l'utilisateur marche pas (tourner)
- R2: Détection des pédales marche pas
- R3: Détection des intreractions inconsistante
- R4: Problèmes de projection
- R5: On arrive pas à utiliser Unreal Engine
- R6: Une personne se blesse durant l'utilisation du projet
- R7: Le vélo stationnaire tombe
- R8: Projection pas clair (trop de lumière)
- R9: un des membre de l'équipe ne peux pas participer pour certaines raisons
- R10: Un bris / usure de matériel
- R11: controle du ventilateur selon la vitesse

Initialement on vas tester Unreal Engine et si on arrive pas à de manière efficace rapidement, on commence à travailler dans unity. (R5)

Nous allons continuer par nous assurer dans les premières semaines que le capteur de mouvement détecte la position de l'utilisateur et retourne une valeur gauche / droite selon la distance par rapport au millieu. (R1) 
Ensuite, nous nous assurerons que la détection de pédales fonctionnent selon la vitesse que l'utilisateur pédale (R2) et que la vitesse de transmission des données ne soit pas inconsistante. (R3)

Selon le lieu, nous allons vérifier l'éclairage (R8) et l'espace nécessaire pour la projection durant la présentation. (R4)

Pour réduire les chances de blessure de l'utilisateur, nous allons tester par nous même des scénario et des possibilité de blessure et nous allons nous informé des information nécessaire avec les gardes. Selon le lieu, nous aurons des garde de sécurité pour nous aider et / ou une personne de notre équipe capable de premier soin mineure. Durant ces test, nous allons voir a quel point une personne peux se pencher avant que le vélo deviennent instable et si le point d'équilibre est trop proche ou restrictif, nous allons trouver une façons de le rendre plus stable.


DESCRIPTION DU PLAN DE TESTS DE RISQUES ICITTE OR SMTH

# Tests à réaliser
## Scénarios
 
| Scénario 1 | L'utilisateur n'a pas encore été détecté par le capteur. Il voit un avant-goût de l'oeuvre par une vidéo en boucle projeter à l'écran.  |
|------------|---|
 
| Identification    | 1.1  Projection déclanché par défault|
|-------------------|---|
| Priorité          | Faible  |
| Date Limite       |   |
| Description       | S'assurer que dès le lancement de l'oeuvre, une vidéo joue en boucle |
| Contraintes       |  |
| Dépendances       | S'assurer que le l'ordinateur et la projection communiquent en harmonie.  |
| Procédure de test |  Données d’entrée : Vidéo de départ Résultats attendus : Projection de la vidéo. Critères de validation : On voit la vidéo. |
| Résultat          |   |
 
| Scénario 2 |  L'utilisateur est détecté par le capteur.|
|------------|---|
 
| Identification    | 2.1  |
|-------------------|---|
| Priorité          |   |
| Date Limite       |   |
| Description       | S'assurer que dès le lancement de l'oeuvre, une vidéo joue en boucle jusqu'à ce qu'un utilisateur soit détecté. S'assurer que si le capteur arrête de capté un utilisateur pour plus de 10 secondes, la vidéo continue ou elle c'était arrêtée.  |
| Contraintes       | Configurer le capteur afin de s'assurer que seulement la présence d'un utilisateur soit détecter.  |
| Dépendances       | S'assurer que le capteur et la projection communiquent en harmonie.  |
| Procédure de test |   Données d’entrée : Vidéo de départ, entrée de l'utilisateur Résultats attendus : Projection de la vidéo interrompu par la présence de l'utilisateur. Critères de validation : Vidéo interrompu, le menu apparâit. |
| Résultat          |   |


# Gestion de problèmes
