# Introduction Markdown
![Markdown](https://cdn0.iconfinder.com/data/icons/octicons/1024/markdown-512.png)

## Définition

*Markdown est un langage de balisage léger créé par John Gruber en 2004. Son but est d'offrir une syntaxe facile à lire et à écrire. Un document formaté selon Markdown devrait pouvoir être publié comme tel, en texte, sans donner l'impression qu'il a été marqué par des balises ou des instructions de formatage.*

>[*source : Wikipedia*](https://www.google.fr/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0ahUKEwjfupHPofHRAhUGWxoKHdJXBVgQFggcMAE&url=https%3A%2F%2Ffr.wikipedia.org%2Fwiki%2FMarkdown&usg=AFQjCNE9raQeaXrHMZzAfAe44MjYxXk3-w&sig2=FRHCXDYk_fDWtKC8iuHbMA&bvm=bv.146073913,d.d2s "Markdown")

## C'est bien joli mais pourquoi en faire ?

**Le Markdown est present** :

* Mail
* Documentation (Sur github)
* Site static

**Le Markdown c'est** :

* Facile à ecrire
* Super leger



## Comment l'écrire ou le lire

---
### Écrire du Markdown
On peut écrire du Markdown avec n'importe quel éditeur de texte, après la coloration syntaxique n'est peut-être pas disponible sur tous.

J'utilise [Atom][atomLink].

---
### Lire du Markdown

On peut lire du Markdown avec [Atom][atomLink], mais aussi sur son navigateur a l'aide d'une extension.

J'utilise [Markdown Reader](https://chrome.google.com/webstore/detail/markdown-reader/gpoigdifkoadgajcincpilkjmejcaanc "download it here"), il gere les **Headers** et en fait un sommaire.


## Modification de texte

---
### Comportement

Le Markdown a besoin d'une ligne de séparation entre deux paragraphes pour les séparer en deux éléments distinctes.

```
Hello I am text
Hello I am still a text

Hello I am a independent

Hello I am still a independent

```

Résultat:

>Hello I am text
>Hello I am still a text
>
> ---
>
>Hello I am a independent
>
>Hello I am still a independent

---
### Gras & Italic

Deux façons de faire
```
*italic*   **bold**
_italic_   __bold__
```
Résultat :   
> *italic*   **bold**
>
> _italic_   __bold__

---
### Headers
Differents types de titres
```
Header 1
=======

Header 2
--------

# Header 1 #
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
 Résultat :
> Header 1
> =======
> Header 2
> --------
> # Header 1 #



## Outils
---
### Liens
Liens classique
```
 [exemple](https://url.com/ "Title")
```

Utilisation :

> My car is a [Ferrari](https://california-t.ferrari.com/ "California T")

Pour un meme liens qui pourrait ce retrouver plusieurs fois dans la même page on utilise des **id**

```
[foo]: http://example.com/  "Optional Title Here"
[foo]: http://example.com/  'Optional Title Here'
[foo]: http://example.com/  (Optional Title Here)

Here the [example][foo]
Go look at the [website][foo]

```

Utilisation :
[atomLink]: https://atom.io/ "the github editor"
> My favorite editor is [Atom][atomLink], you can write and read Markdown with it
>
> You have to [download it][atomLink]

---
### Images

Les images fonctionnent comme les liens. La seule différence est que pour les images il faut rajouter un `!` devant les`[]` qui décrivent l'image

on peut aussi utiliser les **id** pour les images
```
![alt text](/path/img.jpg "Title")
```
Utilisation :
> ![Ferrari](https://california-t.ferrari.com/assets/images/4/Ferrari_tailor_Made_california_blu_post-pontile-718efdb4.jpg "California T")
> ![RedFerrari](https://i.kinja-img.com/gawker-media/image/upload/s--dwklYr1E--/c_scale,fl_progressive,q_80,w_800/ildz2v3kr3vue51opjyq.gif "Gif")

---
### Images avec liens

On a la possibilité de faire des images redirigeant vers des liens.

```
[!["Your picture"](/path/img.jpg)](http://example.com "Your link")

```

Utilisation :

>Cette image redirige vers une voiture
>
>[!["the little picture"](http://logosquiz.net/data/guessthelogo/images/koenigsegg.png)](http://1hosj01irnixn8onr1zmv5s1.wpengine.netdna-cdn.com/wp-content/uploads/2015/03/Regera_Airstrip1.jpg "The big picture")
>*Koenigsegg Regera*



## Listes

---
### Listes à puces & Listes ordonnées

Ces listes peuvent utiliser differents symboles

```
* Unordered list can use asterisks
- Or minuses
+ Or pluses
```
Utilisation :
> To build a website you have to use :
> * HTML
> + CSS
> - Javascript

Les sous-listes sont possible aussi

```
1. First ordered list item
2. Another item
  * Unordered sub-list.
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.

```

Utilisation :
>My favorite cars is :
> 1. Mc Laren
>   * P1
> * Ferrari
>    1. 458 Spider
>    * LaFerrari
> * Jaguar
>    * F-Type
>

---
### Blockquotes
Ils sont utuliser pour les citaions

```
> my quote
```

Utilisation
>> never stop learning, stay curious

---
### BlockCode
Vous permet de faire des blocks dans lequels on peut écrire du code.

>```Javascript
>let liste = [1, 5, 10, 15];
>let doubles = liste.map(x => x * 2)
>```

---
### Lignes Horizontales

```
---

* * *

- - - -
```
Utilisation :
>---

>* * *

>- - - -

---
### To Do
Faire une liste de taches

```
- [ ] Incomplete task
- [x] Task done
```

Utilisation :
> To buy
> - [ ] Milk
> - [x] Water
> - [ ] Vegetable

---
### Tableaux

```
| Header One     | Header Two     |
| :------------- | :------------- |
| Item One       | Item Two       |
```

Utilisation :

| Brand   | Model    | HorsePower | Price (M) | Interior
| :------------- | :------------- | :-------- |:-------- |
| Bugatti | Chiron |   1500  | 2,4 | ![Bugatti][Chiron]
| W Motors | Lykan HyperSport |   750  | 3,4 | ![Lykan HyperSport][LykanHyperSport]

[Chiron]: http://st.motortrend.com/uploads/sites/5/2016/02/2017-Bugatti-Chiron-interior-03.jpg

[LykanHyperSport]: http://www.car-revs-daily.com/wp-content/uploads/2013/12/CarRevsDaily-Supercars-Best-of-2013-W-Motors-Lykan-HyperSport-38.jpg
