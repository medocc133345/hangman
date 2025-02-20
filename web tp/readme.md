# Jeu du Pendu en Go

## Description

Une application web du jeu du pendu développée en Go, utilisant uniquement les packages standards. Les scores sont stockés dans un fichier JSON. L'application propose trois niveaux de difficulté et une interface utilisateur responsive grâce à Bootstrap.

## Fonctionnalités

- **Démarrage d'une nouvelle partie** avec choix de difficulté : Facile, Moyen, Difficile.
- **Interface utilisateur responsive** avec Bootstrap.
- **Gestion des sessions via cookies** encodés en Base64.
- **Fonctionnalité d'indice** pour révéler une lettre non découverte.
- **Enregistrement et affichage des scores** dans un fichier JSON.
- **Page d'erreur 404 personnalisée**.
- **Sécurité renforcée** avec gestion appropriée des cookies.

## Installation

### Prérequis

- [Go](https://golang.org/dl/) installé (version 1.16 ou supérieure recommandée).
- Les images `hangman0.png` à `hangman6.png` placées dans `static/images/`.
- Les mots organisés dans `words/words.txt`.

### Étapes

1. **Cloner le dépôt :**

    ```bash
    git clone https://github.com/medocc133345/web-tp.git
    cd hangman-go
    ```

2. **Organiser les fichiers :**

    Assurez-vous que la structure du projet correspond à celle indiquée dans la [Structure du Projet](#1-structure-du-projet).

3. **Exécuter l'application :**

    ```bash
    go run main.go
    ```

4. **Accéder à l'application :**

    Ouvrez votre navigateur et accédez à [http://localhost:8080](http://localhost:8080).

## Utilisation

1. **Page d'accueil :**

    - Entrez votre pseudo.
    - Choisissez un niveau de difficulté (Facile, Moyen, Difficile).
    - Cliquez sur "Commencer la Partie".

2. **Page de jeu :**

    - Devinez une lettre ou proposez le mot complet.
    - Cliquez sur "Soumettre".
    - Utilisez la fonctionnalité "Obtenir un indice" si nécessaire.

3. **Fin de partie :**

    - Si vous gagnez ou perdez, vous pouvez enregistrer votre score.
    - Cliquez sur "Enregistrer mon score" pour le sauvegarder.
    - Rejouez ou consultez le tableau des scores.

4. **Tableau des scores :**

    - Consultez les scores enregistrés avec les détails des parties.

## Tests

Exécutez les tests unitaires avec :

```bash
go test
#   w e b - t p 1  
 