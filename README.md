# Application Android Compteur

Cette application Android simple permet d'incrémenter un compteur avec un bouton, d'afficher un message via Toast et de réinitialiser le compteur. Elle inclut les fonctionnalités suivantes :
- Un bouton **Toast** qui affiche un message lorsqu'il est cliqué.
- Un bouton **Count** qui incrémente le nombre affiché dans un `TextView` à chaque clic.
- Un bouton **Reset** qui réinitialise le compteur à zéro.

## Fonctionnalités

1. **Bouton Toast** : Lorsque le bouton "Toast" est cliqué, un message Toast apparaît avec le texte "Hello Toast".
2. **Bouton Count** : Chaque fois que le bouton "Count" est cliqué, la valeur du compteur dans le `TextView` est incrémentée de 1.
3. **Bouton Reset** : Lorsque le bouton "Reset" est cliqué, le compteur est remis à zéro.

## Screen Video
[![Vidéo de démonstration]]([video1.webm](https://github.com/user-attachments/assets/a60bcd02-e32b-48e4-90e2-87621d7b3b23)
)

## Explication du code

### MainActivity.java
La logique principale de l'application se trouve dans le fichier `MainActivity.java`. Voici les principaux éléments :

- **Boutons** : 
  - `toast` - Affiche un message Toast.
  - `count` - Incrémente le compteur.
  - `reset` - Réinitialise le compteur à 0.
  
- **TextView** : 
  - `textview` - Affiche la valeur actuelle du compteur.

Les méthodes suivantes gèrent les événements de clic sur les boutons :

- `toast.setOnClickListener` : Affiche un message Toast disant "Hello Toast".
- `count.setOnClickListener` : Incrémente le compteur (`currentCount`) et met à jour le `TextView` avec la nouvelle valeur.
- `reset.setOnClickListener` : Réinitialise le compteur à zéro et met à jour le `TextView`.

### activity_main.xml
Ce fichier définit la disposition de l'application :
- Un `TextView` pour afficher la valeur du compteur.
- Trois boutons pour les fonctionnalités Toast, Count et Reset.
- La disposition est un `LinearLayout` vertical avec des marges et des espacements adéquats.

## Comment exécuter l'application

1. Clonez ce dépôt ou téléchargez le code source.
2. Ouvrez le projet dans Android Studio.
3. Compilez et lancez l'application sur un appareil Android ou un émulateur.

## Dépendances

- Android SDK 21 ou supérieur.
- Java 8 ou supérieur.
