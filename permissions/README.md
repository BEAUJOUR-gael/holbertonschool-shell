# Shell, Permissions

Ce dossier contient des scripts permettant de manipuler les permissions, les utilisateurs et les groupes sur Linux.

## Liste des scripts

### `0-iam_betty`
> Change l’utilisateur courant pour l’utilisateur **betty**.

**Commande utilisée :**
```bash
su betty
### `1-who_am_i`
> Affiche le **nom de l’utilisateur effectif** courant.

**Commande utilisée :**
```bash
whoami
### `2-groups`
> Affiche tous les **groupes** dont l’utilisateur courant fait partie.

**Commande utilisée :**
```bash
groups
### `3-new_owner`
> Change le **propriétaire** du fichier `hello` pour le rendre appartenant à l’utilisateur **betty**.

**Commande utilisée :**
```bash
chown betty hello
### `4-empty`
> Crée un fichier vide nommé **hello**.

**Commande utilisée :**
```bash
touch hello
### `5-execute`
> Ajoute la **permission d’exécution** au **propriétaire** du fichier `hello`.

**Commande utilisée :**
```bash
chmod u+x hello
### `6-multiple_permissions`
> Ajoute plusieurs permissions au fichier `hello` :
> - **Exécution (x)** pour le **propriétaire (u)**  
> - **Exécution (x)** pour le **groupe (g)**  
> - **Lecture (r)** pour les **autres utilisateurs (o)**

**Commande utilisée :**
```bash
chmod ug+x,o+r hello
### `7-everybody`
> Ajoute la **permission d’exécution** à **tous les utilisateurs** (owner, group, others) pour le fichier `hello`.

**Commande utilisée :**
```bash
chmod a+x hello
### `8-James_Bond`
> Définit les permissions du fichier `hello` :
> - Owner : aucune permission  
> - Group : aucune permission  
> - Others : lecture, écriture et exécution (`rwx`)

**Commande utilisée :**
```bash
chmod 007 hello
### `9-John_Doe`
> Définit les permissions du fichier `hello` comme suit :  
> `-rwxr-x-wx`  
> - Owner : lecture, écriture, exécution  
> - Group : lecture, exécution  
> - Others : écriture, exécution

**Commande utilisée :**
```bash
chmod 753 hello
### `10-mirror_permissions`
> Définit les permissions du fichier `hello` pour qu’elles soient **identiques à celles de `olleh`**.

**Commande utilisée :**
```bash
chmod --reference=olleh hello
