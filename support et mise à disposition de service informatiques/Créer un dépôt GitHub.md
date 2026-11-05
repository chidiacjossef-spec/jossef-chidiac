# Procédure : Créer un dépôt GitHub

Cette procédure décrit les étapes pour initialiser un nouveau dépôt sur GitHub et y lier un projet local en ligne de commande.

## Prérequis
* Un compte GitHub actif.
* L'outil `git` installé sur votre machine locale.

---

## Étape 1 : Création du dépôt sur GitHub
1. Connectez-vous à votre compte sur **GitHub**.
2. Dans le coin supérieur droit, cliquez sur le bouton **`+`** puis sélectionnez **New repository**.
3. Remplissez les informations suivantes :
	* **Repository name** : Saisissez le nom de votre projet.
	* **Public/Private** : Choisissez la visibilité de votre dépôt.
4. Laissez les options *README*, *.gitignore* et *License* décochées (elles seront initialisées localement).
5. Cliquez sur le bouton vert **Create repository**.

---

## Étape 2 : Initialisation et liaison en local
Ouvrez votre terminal (Linux/macOS) ou PowerShell (Windows) dans le dossier de votre projet, puis exécutez les commandes suivantes :

1. **Initialiser le dépôt Git local :**
```bash
git init
```

2. **Ajouter les fichiers du projet à l'index :**
```bash
git add .
```

3. **Valider les fichiers avec un premier commit :**
```bash
git commit -m "Initial commit"
```

4. **Renommer la branche principale en `main` :**
```bash
git branch -M main
```

5. **Lier le dossier local au dépôt distant sur GitHub :**
*(Remplacez l'URL ci-dessous par celle fournie par GitHub)*
```bash
git remote add origin https://github.com
```

6. **Pousser le projet vers GitHub :**
```bash
git push -u origin main
```

---

## Étape 3 : Vérification
1. Retournez sur la page de votre dépôt sur GitHub.
2. Actualisez la page.
3. Vérifiez que l'arborescence de vos fichiers locaux apparaît correctement en ligne.