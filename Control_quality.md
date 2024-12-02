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
- R5: On arive pas à utiliser Unreal Engine
- R6: L'utilisateur se blesse
- R7: Le vélo stationnaire tombe
- R8: Projection pas clair (trop de lumière)
- R9: Un d'entre nous échoue un cours

Nous allons nous assurer dans les premières semaines que la caméra détecte la position de l'utilisateur et retourne une valeur gauche / droite selon la distance par rapport au millieu. (R1) Nous allons en même 

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
