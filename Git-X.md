# Git ![x](./src/img/X-icons8.com.png)

Bienvenue dans le rapport **Git X**.

**Git X** fait des e**X**périmentations et note ses différentes actions dans ce rapport !

À Nous de le construire.

****
## **@Wyllem** -- *02/03/2017* :

> On a fait un dépôt distant avec un dossier `REMOTE` et un dépôt local avec un dossier `Working` qui communiquent. Le `REMOTE` reçoit les changement fait dans le `Working`.

> Pour cela on a creer un dépôt distant :

> * `$ mkdir REMOTE`
-- *Creation du dossier*
> * `$ git init --bare`
-- *Initialisation du dépôt distant*
> * `$ git remote add origin <url>`
-- *Creation du dépôt*
> * `$ git remote -v`
-- *Visualiser l'url et le nom du remote*

> Et aussi un dépôt local (A l'exterieur du dépôt `REMOTE`, n'importe où dans le pc) :

> * `$ mkdir Working`
-- *Creation du dossier*
> * `$ git init`
-- *Initialisation du dépôt local*
> * `$ git remote add origin <Même_url>`
-- *Liaison au dépôt*
> * `$ git remote -v`
-- *Visualiser l'url et le nom du remote*

> Les deux dossier sont liés on peut faire des commit 😁

> On a créer un fichier vide: `touch index.html`

> On l'a stage (zone de transit)  avec : `git add index.html`

> Commit avec : `git commit -m "Initial commit"`

> Et envoyer les changement au `REMOTE` avec : `git push origin master`

> Si on se rend sur le `REMOTE` et que on fait un `git log --oneline` on obtient :
`c5f908a initial Commit`
