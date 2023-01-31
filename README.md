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



<img width="1130" alt="access log" src="https://user-images.githubusercontent.com/122889266/215875887-dbacd8c7-0184-4d5f-8a04-687ebc190b19.png">




error.log

<img width="642" alt="error komento" src="https://user-images.githubusercontent.com/122889266/215875861-e27d3b32-ea1a-4b1e-a1d8-a455f33b1c0b.png">




Onnistunut tapahtuma lokiin 

Kokeilin sammuttaa koneeltani verkkoyhteyden ja testasin näkyisikö se lokissa. 

Sain alla olevan mukaisen kuvan, josta näkee, että verkkoyhteys on katkaistu. 

Seuraavassa kuvassa näkyy, että verkkoyhteys toimii taas. 

<img width="811" alt="Yhteys toimii" src="https://user-images.githubusercontent.com/122889266/215861686-2a640d15-01d4-4f71-bb6d-74b18ebc867a.png">

Seuraavaksi yritin aiheuttaa epäonnistuneen tapahtuman lokiin. Yritin antaa väärän salasanan komennolle sudo cat syslog ja katsoin auth.log näkyisikö tapahtuma. Alla testin tulos.


<img width="809" alt="Yhteys ei toimi" src="https://user-images.githubusercontent.com/122889266/215875716-791dc65c-c125-430d-baea-3e49391034ee.png">
<img width="809" alt="Auth tulostus" src="https://user-images.githubusercontent.com/122889266/215875735-5f253194-537a-4855-932f-bd5ac6f4e896.png">
<img width="601" alt="Auth komento" src="https://user-images.githubusercontent.com/122889266/215875744-91a24e80-c43c-4d9d-b784-25e7aed41c68.png">
<img width="552" alt="Syslog komento" src="https://user-images.githubusercontent.com/122889266/215875754-6457bc25-b587-4db3-87ec-75ca94a334e9.png">
<img width="803" alt="Syslog tulos2" src="https://user-images.githubusercontent.com/122889266/215875832-e6bf16a7-bfc0-4a41-906d-d2cab01b9288.png">






Onnistunut tapahtuma lokiin 

Kokeilin sammuttaa koneeltani verkkoyhteyden ja testasin näkyisikö se lokissa. 

Sain alla olevan mukaisen kuvan, josta näkee, että verkkoyhteys on katkaistu. 

Seuraavassa kuvassa näkyy, että verkkoyhteys toimii taas. 

Epäonnistunut tapahtuma lokiin



Seuraavaksi yritin aiheuttaa epäonnistuneen tapahtuman lokiin. Yritin antaa väärän salasanan komennolle sudo cat syslog ja katsoin auth.log näkyisikö tapahtuma. Alla testin tulos.









