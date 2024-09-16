
```mermaid
flowchart TD
    A[Veille] -->|Interaction| C(Menu)
    C -->|Jouer| D[Commence le jeu]
    C -->|Consignes| E[Affiche Consignes]
    C -->|Quitter| F[Quitter l'expérience]
    F --> A
    E[Affiche Consignes]--> |Menu| C[Menu]
    D --> H{Niveau1}
  ```
