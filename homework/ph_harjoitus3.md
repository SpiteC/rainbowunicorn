# Palvelinten Hallinta - Harjoitus 3

`echo "Testing this markdown down."`


## z) Lue ja tiivistä


[Commonmark contributors: Markdown Reference](https://commonmark.org/help/)

* Koottu esimerkkilista markdownin formatoinnista
* Headings, code inline/block, link, image
* 10 minuutin tutoriaalilinkki


## a) MarkDown. Tee tämän tehtävän raportti MarkDownina. Helpointa on tehdä raportti GitHub-varastoon, jolloin md-päätteiset tiedostot muotoillaan automaattisesti. Tyhjä rivi tekee kappalejaon, risuaita ‘#’ tekee otsikon, sisennys merkitsee koodinpätkän.


Aloitin harjoituksen luomalla virutaalikoneelleni uuden SSH avaimen kuten tunnilla käytiin läpi, jotta voisin kloonata luodun repon omalle koneelleni sen avulla.

`ssh-keygen -r ecdsa -C "pyry.rauhala@myy.haaga-helia.fi"`

Komennossa luodaan siis uusi ecdsa -avain sen hetkiseen hakemistoon ja lopussa annan sähköpostiosoitteen. Komento luo avaimen .ssh hakemistoon, joka piilotettu normaalinäkymästä. Tämän jälkeen kopioin luodun .pub avaimen githubin asetuksiin ja kloonasin repon SSH linkillä seuraavaan tapaan:

`git clone git@github.com:SpiteC/rainbowunicorn.git`

Kun repo oli kloonattu, navigoin sen hakemistoon ja loin sinne uuden "homework" hakemiston ja tämän .md tiedoston. Testasin muutaman kerran alkuun miten formatointi toimii ja pienen harjoittelun jälkeen kaikki perushommat olivatkin jo hallussa.


## b) Pull first. Tee useita muutoksia git-varastoosi. Tee muutama muutos, jossa yksi commit koskee useampaa tiedostoa. Anna hyvä kuvaukset (commit message), yksi englanninkielinen lause imperatiivissa (määräysmuodossa) "Add top level menu to Foobar synchronizer"


Tässä tehtävässä loin uuden kansion nimeltä "pictures", jonne aion tallettaa kuvankaappaukset tätä tehtävää varten. Kuvankaappauksia varten asensin iamgemagick nimisen työkalun.

```
mkdir pictures
sudo apt-get -y install imagemagick
```

Seuraavaksi loin työkalulla kuvankaappauksen työpöydästä ja tallensin sen pictures kansioon. Lisäsin kuvan myös tähän, jolla sain useamman muutoksen gittiin.

![Kuva1](./pictures/h3_pic1.png)

## Lähteet:

CommonMark Help Page: Commonmark contributors: Markdown Reference. https://commonmark.org/help/

Roger Dudler, 2015: git - the simple guide. https://rogerdudler.github.io/git-guide/
