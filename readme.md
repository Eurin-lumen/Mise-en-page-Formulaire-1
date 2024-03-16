Le CSS est utilisé pour styliser et mettre en forme le formulaire de contact que nous avons créé dans le fichier HTML `contact.html`. Voici une explication détaillée du CSS utilisé dans le fichier `styles.css` :

1. **Body et Reset CSS**:
```css
body {
    font-family: Arial, sans-serif;
    background-color: #f7f7f7;
    margin: 0;
    padding: 0;
}
```
- `font-family` : Définit la police de caractères utilisée dans tout le document.
- `background-color` : Définit la couleur de fond de la page.
- `margin` et `padding` : Supprime les marges et les rembourrages par défaut du corps de la page.

2. **Conteneur principal**:
```css
.container {
    max-width: 600px;
    margin: 50px auto;
    padding: 20px;
    background-color: #fff;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
```
- `max-width` : Limite la largeur du conteneur à 600 pixels maximum.
- `margin` : Centre le conteneur horizontalement avec un espace de 50 pixels en haut et en bas.
- `padding` : Ajoute un espace intérieur de 20 pixels au contenu du conteneur.
- `background-color` : Définit la couleur de fond du conteneur.
- `border-radius` : Arrondit les coins du conteneur.
- `box-shadow` : Ajoute une ombre légère au conteneur pour le faire ressortir.

3. **Titre du formulaire**:
```css
h2 {
    color: #333;
    text-align: center;
    margin-bottom: 20px;
}
```
- `color` : Définit la couleur du texte.
- `text-align` : Centre le texte horizontalement.
- `margin-bottom` : Ajoute un espace en bas du titre.

4. **Groupes de champs d'entrée**:
```css
.input-group {
    margin-bottom: 15px;
}
```
- `margin-bottom` : Ajoute un espace en bas de chaque groupe de champ d'entrée.

5. **Étiquettes (labels)**:
```css
label {
    display: block;
    margin-bottom: 5px;
    color: #333;
}
```
- `display: block` : Fait en sorte que les étiquettes soient affichées sur une ligne séparée.
- `margin-bottom` : Ajoute un petit espace en bas de chaque étiquette.
- `color` : Définit la couleur du texte de l'étiquette.

6. **Champs de texte, d'email et zone de texte**:
```css
input[type="text"],
input[type="email"],
textarea {
    width: 100%;
    padding: 10px;
    border-radius: 3px;
    border: 1px solid #ccc;
}
```
- `width: 100%` : Fait en sorte que les champs de texte et la zone de texte occupent toute la largeur du conteneur.
- `padding` : Ajoute un espace intérieur de 10 pixels aux champs.
- `border-radius` : Arrondit les coins des champs.
- `border` : Ajoute une bordure de 1 pixel solide de couleur grise.

7. **Bouton Envoyer**:
```css
button {
    display: block;
    width: 100%;
    padding: 10px;
    border: none;
    background-color: #007bff;
    color: #fff;
    border-radius: 3px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}
```
- `display: block` : Affiche le bouton sur une ligne séparée.
- `width: 100%` : Fait en sorte que le bouton occupe toute la largeur du conteneur.
- `padding` : Ajoute un espace intérieur de 10 pixels au bouton.
- `border: none` : Supprime la bordure du bouton.
- `background-color` : Définit la couleur de fond du bouton.
- `color` : Définit la couleur du texte du bouton.
- `border-radius` : Arrondit les coins du bouton.
- `cursor: pointer` : Affiche le curseur en forme de main au survol du bouton.
- `transition` : Ajoute une transition en douceur lors du changement de couleur de fond du bouton.

8. **Validation des champs obligatoires**:
```css
input:invalid,
textarea:invalid {
    border-color: #dc3545;
}

input:invalid:focus,
textarea:invalid:focus {
    box-shadow: 0 0 5px #dc3545;
}
```
- `input:invalid` et `textarea:invalid` : Applique un style lorsque les champs obligatoires ne sont pas remplis.
- `border-color` : Définit la couleur de la bordure en cas de champ invalide.
- `input:invalid:focus` et `textarea:invalid:focus` : Applique un style lorsque l'utilisateur met le focus sur un champ invalide.
- `box-shadow` : Ajoute une ombre autour du champ invalide pour attirer l'attention de l'utilisateur.