# A 2019-es magyarországi EP választások eredményeinek elemzése

*Gyarmathy Zsófia, 2019. június*

## Rövid összefoglaló

A 2019-es magyarországi EP választásokon a pártok által elért eredményeket elemeztem különböző mutatók függvényében. 

**Az elemzés a következő linken tekinthető meg:**
**<https://nbviewer.jupyter.org/github/gyarmathy/EPvalasztasHU2019/blob/master/valasztasi_adatok_elemzese.ipynb>**

## Felhasznált adatok
 
Az elemzés eredményeit grafikonok és interaktív korrelációs táblák formájában
a [valasztasi_adatok_elemzese Jupyter jegyzetfüzet](valasztasi_adatok_elemzese.ipynb) tartalmazza.
 
Az elemzéshez csak szabadon hozzáférhető adatokat használtam (az adatok forrásainak linkjét a fenti jegyzetfüzet tartalmazza, 
az eredeti adatokat pedig a [datain](datain) könyvtár):
1. a választási eredményeket a valasztas.hu oldaláról ([EP_2019_szavazóköri_eredmény.xlsx](datain/EP_2019_szavazóköri_eredmény.xlsx));
2. a KSH területi adatait (a többi fájl a [datain](datain) könyvtárban).
    * A KSH adatfelhasználási tájékoztatója [ezen a inken elérhető](https://www.ksh.hu/docs/szolgaltatasok/adatigenyles/felhasznalasi_feltetelek_nyilvanos_mikroadatfajlok.pdf).
3. A választási eredményeket elemző szkript letölt és kicsomagol egy `datamap` nevű mappába egy szabadon felhasználható, ám engedély nélkül nem terjeszthető térképalakfájlt a <https://gadm.org/> oldalról.

A fenti forrásokból nyert adatokból három adatfájlt készítettem elő az elemzéshez, amelyek a
[dataout](dataout) könytárban találhatók:
* [valasztasi_eredmenyek](dataout/valasztasi_eredmenyek.csv): a választási eredmények; 
    * forrásszkript: [valasztasi_adatok.ipynb](valasztasi_adatok.ipynb) szkript
* [helyisegnevkonyv](dataout/helyisegnevkonyv.csv): település szintű KSH adatok; 
    * forrásszkript: [helyisegnev_adatok.ipynb](helyisegnev_adatok.ipynb)
* [megyei_adatok](dataout/megyei_adatok.csv): megyei szintű KSH adatok; 
    * forrásszkript: [megyei_adatok.ipynb](megyei_adatok.ipynb)
    
Az elemzéshez használt további segédszkriptek a főkönyvtárban:
* [definitions.ipynb](definitions.ipynb): általános Python csomagimportok és definíciók.
* [valasztasi_adatok_elemzese_01_adatimport.ipynb](valasztasi_adatok_elemzese_01_adatimport.ipynb): 
a [valasztasi_adatok_elemzese.ipynb](valasztasi_adatok_elemzese.ipynb) által használt szkript.

Az elemzés bármilyen célra szabadon felhasználható a szerző megadása mellett.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

Copyright (C) 2019 Zsofia Gyarmathy
