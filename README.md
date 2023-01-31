# Harjoitus4
Tiivistelmä artikkelista


Tukki

a)	analysoi


/var/log/syslog

Komento

Tulostus








Systemd-hostname service. En suoraan ymmärtänyt mitä tämä tarkoittaa. Löysin jonkun lähteen, mutta en ymmärtänyt oikein senkään avulla. 

https://www.freedesktop.org/software/systemd/man/systemd-hostnamed.service.html


Auth.log


access.log




error.log




Onnistunut tapahtuma lokiin 

Kokeilin sammuttaa koneeltani verkkoyhteyden ja testasin näkyisikö se lokissa. 

Sain alla olevan mukaisen kuvan, josta näkee, että verkkoyhteys on katkaistu. 

Seuraavassa kuvassa näkyy, että verkkoyhteys toimii taas. 

<img width="811" alt="Yhteys toimii" src="https://user-images.githubusercontent.com/122889266/215861686-2a640d15-01d4-4f71-bb6d-74b18ebc867a.png">

Seuraavaksi yritin aiheuttaa epäonnistuneen tapahtuman lokiin. Yritin antaa väärän salasanan komennolle sudo cat syslog ja katsoin auth.log näkyisikö tapahtuma. Alla testin tulos.





