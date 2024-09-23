# Projet: 

## Idée
Course de véhicule style Nascar

## Objectif
La vitesse du vélo stationnaire définit la vitesse du véhicule, plus l’utilisateur pédale vite, plus le véhicule accélèrent et le contraire se produit si l’utilisateur ralentit ou arrête de pédaler.

On peut retrouver un frein relié à un moteur qui peut ralentir rapidement l’utilisateur et le véhicule.

Sur chaque côté des poignées se trouvent des boutons qui permettent de tourner à droite et à gauche.

Il y a un garage permettant de faire des améliorations aux véhicules et même de changer de véhicules.

Dans la course, il y a plusieurs événements aléatoires et programmés comme la conduite des autres véhicules dans la course, des accidents qui peuvent bloquer la route, des événements météorologiques comme de la pluie ou du vent, l’usure des pneus pourrait rendre le véhicule plus instable, il faudrait alors aller au pit stop pour les changer.

Collision avec autres véhicules activés.

Plusieurs pistes de course différentes demandant véhicules, pièce et conduite différente.

Il y aurait aussi un bouton à gauche permettant de changer de caméra de véhicule et un a droite permettant d’activer un turbo temporaire.
Easter Egg permettant d’avoir des power-up ou véhicule unique


## Scénario
```mermaid
flowchart TD
    A[Veille] -->|Interaction| C(Menu)
    C -->|Jouer| D[Commence le jeu]
    C -->|Consignes| E[Affiche Consignes]
    C -->|Quitter| F[Quitter l'expérience]
    F --> A
    E[Affiche Consignes]--> |Menu| C[Menu]
    D --> H{Course1}
    D --> I{Garage}
    I --> C
    H --> J{Course2}

  ```
