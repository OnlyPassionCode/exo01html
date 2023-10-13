# Création d'un dépôt GIT

## Création d'un dépôt GIT en local

Dans la console, initialisation du dépôt: 

```bash
git init
```
## Visualisation de l'état de GIT

```bash
git status
```
### Pour voir les fichiers et dossiers Unix

```bash
ls -a
```
## Pour ajouter un fichier à la future sauvegarde

```bash
git add <nameFile>
git add README.md
```

## Pour effectuer la sauvegarde

Les fichiers en attentes de sauvegarde sont en vert.

Les fichiers non suivi sont en rouge.

Seul les fichiers en **staging** seront sauvés

```bash
git commit -m "Message du commit"
```
Un commit est une sauvegarde, on peut y accèder 
avec un `git log` (affichage des identifiants des sauvegardes 
et `git show` (sans paramètre, affichage du dernier commit)

## Pour ajouter tous les fichiers en staging

```bash
git add .
```
## Ajout d'un serveur distant

Nous allons utiliser un dépôt que l'on va créer sur github.com,
après connexion. Comme c'est un travail personnel, son URL sera 
de ce type : https://github.com/VOTRE_USERNAME/leNomDuProjet

Nous créons un new Repository, puis nous copions la clé SSH : 

git@github.com:OnlyPassionCode/exo01html.git

Nous retournons dans notre git bash :

```bash
git remote add origin git@github.com:OnlyPassionCode/exo01html.git
```
Pour voir si ça a fonctionné :

```bash
git remote -v
```
