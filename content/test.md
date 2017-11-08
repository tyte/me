---
views:            
    byline:
            region: after-main
            template: default/content
            sort: 1
            data:
                meta:
                    type: content
                    route: block/byline
...

Testsida
==============================================

Här testar jag Markdown.


Länkning till sidor {#url}
---------------------------------

Länkar är relativa. Jag behöver endast veta var rooten finns. Här använder vi [`htdocs`]()

Länk till en fil i samma katalog: [license.md](license).
Länk till en fil i annan katalog: [report/kmom01](report/kmom01).



Länk till en bild {#img}
---------------------------------

Liknar länkning till vanliga sidor.


```text
Markdown version: ![igelkott](img/igelkott.jpg)
html version: <img src="img/igelokott.jpg" alt="igelkott">
```
Resultat av koden ovan:

![igelkott](img/igelkott.jpg)
<img src="img/igelkott.jpg" alt="igelkott">


Referenslänkar
-----------------

Text:
```text
I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"
```

Resultat:

I get 10 times more traffic from [Google] [1] than from
[Yahoo] [2] or [MSN] [3].

  [1]: http://google.com/        "Google"
  [2]: http://search.yahoo.com/  "Yahoo Search"
  [3]: http://search.msn.com/    "MSN Search"

Läkning till assets/resources {#asset}
---------------------------------


1. Använd [enkla relativa länkar](dbwebb.se/anax/snygga-lankar). Basurl kommer läggas till automatiskt i början av länken.

2. Lägger man till `!` får man ingen automatiskt basurl i början av länken.

Exempel av relativ länk till en bild:
```text
[Se bilden i storformat](!img/dbwebbisar.jpg)
<a href="!img/dbwebbisar.jpg">
    <img src="img/dbwebbisar.jpg" alt="alt text">
</a>
```
Resultat:
[Se bilden i storformat](!img/dbwebbisar.jpg)
<a href="!img/dbwebbisar.jpg">
    <img src="img/dbwebbisar.jpg" alt="alt text">
</a>



Skapa en mailto: länk {#mailto}
---------------------------------

Så ser det ut när du skriver:
```text
<mailto:user@example.com>
<user@example.com>
<a href="mailto:user@example.com">user@example.com</a>
```

Resultatet:

* <mailto:user@example.com>
* <user@example.com>
* <a href="mailto:user@example.com">user@example.com</a>

Rubriker
---------------------------------

# H1

## H2

### H3

#### H4

##### H5

###### H6

Citat
--------------------

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Listor
----------------

*   Red
*   Green
*   Blue

1.  Bird
2.  McHale
3.  Parish

*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.

Textelement
-------------

Em: *single asterisks*

Strong: **double asterisks**

Tabeller
-----------

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

Definitionslistor
------------------

Apple
:   Pomaceous fruit of plants of the genus Malus in
    the family Rosaceae.

Orange
:   The fruit of an evergreen tree of the genus Citrus.

Fotnot
-----------

That's some text with a footnote.[^1]
That's some text with a footnote.[^2]

[^1]: And that's the footnote.
[^2]: And that's the footnote.

Förkortningar
-------------

The HTML specification
is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]:  World Wide Web Consortium
