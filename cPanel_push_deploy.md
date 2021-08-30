# cPanel push deploy

cPanel pruža mogućnost automatskog pokretanja deploy funkcije za sve git repozitorije koje se hostuju na cPanel serveru. Da bi se ovo postiglo, neophodno je da lokalni git repozitorijum sadrži `.cpanel.yml` fajl i da bude podešena autentifikacija lokalnog računara putem ssh ključa. Takođe je neophodno da na lokalnom računaru bude instaliran [git](https://git-scm.com/downloads).

## Deploy fajl
Deploy fajl `.cpanel.yml` u sebi sadrži listu naredbi koje treba da budu pokrenute onda kada se nove izmene dodaju u repozitorijum, odnosno onda kada korisnik sa svog računara pokrene komandu `git push` Ovo ne mora da se odnosi samo na sinhronizaciju sa javno dostupnim direktorijumom ali se za to najčešće koristi.

## Postupak za kreiranje git repozitorijuma na cPanel-u

Prvi korak jeste kreiranje SSH ključa na lokalnom računaru. Za detalje o ovom koraku možete pročitati povezani članak: [Generisanje SSH ključeva](https://www.dreamclients.com/help/kb/article/cpanel/generisanje-ssh-kljuceva) i [SSH pristup serveru](https://www.dreamclients.com/help/kb/article/cpanel/ssh-pristup-serveru)

Sledeći korak jeste kreiranje git repozitorijuma.