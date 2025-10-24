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
