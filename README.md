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

4 Folder sadrzi tzv. faild runs, tj. pokusaje treniranje koje nisu dosegel zeljenu tacnost (hence njihov naziv). Nisu namenjni za pokretanje, vise kao primer, jer su radjeni bez regularizacije.

## Skup podataka i obuceni modeli
Zbog nemogucnosti da se uploaduju modeli i skup podataka, isti su dostupno na: https://drive.google.com/drive/folders/1gzkktVM-l9amugXDLynvR7WpCbIIou1x?usp=sharing

trained_models.zip i tiny-imagenet-200-modified-testholdout.zip treba raspakovati u folderu gde su svekse za evaluaciju. Takoodje pre pokretanja treba kreirati evaluation_results folder za cuvanje slika. 

tiny-imagenet-200-modified.zip sadrzi folder za treniranje i testiranje

## Literatura
Github nije dozvolio nekeda se uploaduju, iz nepoznatog razloga, pa su uploadovani takodje na drive.

[1] - Residual Attention Networks for Image Classification - Thaminda Edirisooriya
[2] - A ConvNet for the 2020s - Liu et al.
[3] - An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale - Dosovitskiy et al.
[4] - Swin Transformer: Hierarchical Vision Transformer using Shifted Windows - Liu et al.
[5] - Training data-efficient image transformers & distillation through attention - Touvron et al.
[6] - Vision Transformers in 2022: An Update on Tiny Imagenet - Ethan M. Huynh


