
```mermaid
flowchart TD
    A[Veille] -->|Interaction| B(Menu Principal)
    B --> C{Let me cook}
    C -->|Jouer| D[Commence le jeu]
    C -->|Consignes| E[Affiche Consignes]

    C -->|Quitter| F[Quitter l'expérience]
  E[Affiche Consignes]--> |Menu| C[Menu]
 
  ```
