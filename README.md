# -Poređenje konvolutivnih i attention zasnovanih arhitektura za klasiﬁkaciju slika

Rad poredi arhitekture zasnovane na konvoluciji i konceptu paznje.
Obucena su tri podela ConvNeXt kao predstavnik konvolucije. I dva modela kao predstavnici za paznju Vison transformer i Swin transformer.

## Skup podataka
Skup podataka je modifikovan tiny-imagenet-200.
Modifikacije se sastoje od menjnje strukture val radi lakseg ucitavanja.
Izbacivanje 25 slika po klasi iz trening skupa da bi se napravio holout set od 5000 slika. Originalni skup podatak nije imao klase asocirane sa test slikama.

## Folderi
1 Folder sadrzi svesku gde se analizira skup podatak koji se koisiti za trening i validaciju,
2 Folder sadrzi 3 sveske, svaka je za po jedan model. Svekse predstavljaju nootbooks u stanju nakon treniranja model. Modeli su trenirani na Google Colabu. Samim tim i putanje su u odnsu na to okruzenje.
3 Folder sadrzi 3 sveske. Prva sveka racuna metrike na test skupu za Convnext model. Druga sveska za Vit i Swin modele. Prva i druga sveska generisu .json fajlove gde su zapisane metrike. Treca sveska pravi poredjenja i generise grafikone, koji su sacuvani u odgovarajucem folderu.

## Skup podataka i obuceni modeli
Zbog nemogucnosti da se uploaduju modeli i skup podataka, isti su dostupno na: https://drive.google.com/drive/folders/1gzkktVM-l9amugXDLynvR7WpCbIIou1x?usp=sharing
