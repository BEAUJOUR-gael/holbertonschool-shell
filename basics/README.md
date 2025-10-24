# Shell Basics - Scripts

Ce dossier contient les scripts Bash permettant de manipuler le shell et d’apprendre les bases de Linux.

## Liste des scripts

### `0-current_working_directory`
> Affiche le **chemin absolu du répertoire de travail actuel**.

**Commande utilisée :**  
```bash
pwd
### `1-listit`
> Affiche la **liste du contenu du répertoire courant**.

**Commande utilisée :**  
```bash
ls
### `2-bring_me_home`
> Change le répertoire de travail pour aller dans le **dossier personnel de l’utilisateur**.

**Commande utilisée :**
```bash
cd ~
### `3-listfiles`
> Affiche le contenu du répertoire courant en **format long**.

**Commande utilisée :**
```bash
ls -l
### `4-listmorefiles`
> Affiche le contenu du répertoire courant **en format long**, y compris les **fichiers cachés**.

**Commande utilisée :**
```bash
ls -la
### `5-listfilesdigitonly`
> Affiche le contenu du répertoire courant :
> - en **format long**  
> - en **incluant les fichiers cachés**  
> - avec les **UID et GID numériques**

**Commande utilisée :**
```bash
ls -lan
### `6-firstdirectory`
> Crée un dossier nommé **my_first_directory** dans le répertoire **/tmp/**.

**Commande utilisée :**
```bash
mkdir /tmp/my_first_directory
### `7-movethatfile`
> Déplace le fichier **betty** du dossier **/tmp/** vers **/tmp/my_first_directory/**.

**Commande utilisée :**
```bash
mv /tmp/betty /tmp/my_first_directory/
### `8-firstdelete`
> Supprime le fichier **betty** situé dans **/tmp/my_first_directory/**.

**Commande utilisée :**
```bash
rm /tmp/my_first_directory/betty
### `9-firstdirdeletion`
> Supprime le dossier **my_first_directory** situé dans **/tmp/**.

**Commande utilisée :**
```bash
rmdir /tmp/my_first_directory
nano README.md
### `11-lists`
> Affiche en **format long** et inclut les **fichiers cachés** des répertoires :
> - le répertoire courant (`.`)
> - le répertoire parent (`..`)
> - le répertoire `/boot`

**Commande utilisée :**
```bash
ls -la . .. /boot
nano README.md

### `13-symbolic_link`
> Crée un **lien symbolique** nommé `__ls__` pointant vers `/bin/ls`, dans le répertoire courant.

**Commande utilisée :**
```bash
ln -s /bin/ls __ls__
### `14-copy_html`
> Copie tous les fichiers **.html** du dossier courant vers le **dossier parent**,  
> uniquement si le fichier **n’existe pas** ou si la version source est **plus récente**.

**Commande utilisée :**
```bash
cp -u *.html ..
### `15-lets_move`
> Déplace tous les fichiers dont le **nom commence par une majuscule** vers le dossier **/tmp/u/**.

**Commande utilisée :**
```bash
mv [A-Z]* /tmp/u/
