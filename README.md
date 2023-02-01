# Harjoitus4



Tukki


/var/log/syslog

Ensin tutkin syslog tiedostoa alla olevalla komennolla.

<img width="552" alt="Syslog komento" src="https://user-images.githubusercontent.com/122889266/215875754-6457bc25-b587-4db3-87ec-75ca94a334e9.png">

Tulostuksesksi sain:

<img width="803" alt="Syslog tulos2" src="https://user-images.githubusercontent.com/122889266/215875832-e6bf16a7-bfc0-4a41-906d-d2cab01b9288.png">



Ensin näkyy päivämäärä ja kellonaika. Sitten näkyy tietokoneen nimi ja järjestelmänhallinta. Seuraavaksi näkyy tulostus: systemd-hostname.service. En suoraan ymmärtänyt mitä tämä tarkoittaa. Yritin tulkita tulostusta lähteen avulla, mutta siitä huolimatta en ihan ymmärtänyt tulostuksen merkitystä. 

https://www.freedesktop.org/software/systemd/man/systemd-hostnamed.service.html


var/log/auth.log

Seuraavaksi analysoin var/log/auth.log tiedoston sisältöä. Alla näkyy kometo, jolla pääsin katsomaan tiedostoa. 

<img width="601" alt="Auth komento" src="https://user-images.githubusercontent.com/122889266/215875744-91a24e80-c43c-4d9d-b784-25e7aed41c68.png">



<img width="809" alt="Auth tulostus" src="https://user-images.githubusercontent.com/122889266/215875735-5f253194-537a-4855-932f-bd5ac6f4e896.png">


Tulostuksessa näkyy ensin päivämäärä ja kellonaika. Sitten näkyy tietokoneen nimi. Sitten näkyy järjestelmään sisäänkirjautuminen ja että sisään kirjautui käyttäjä Noora. Hakasuluissa oleva 480 [480] merkitys jäi epäselväksi.

/var/log/apache2/access.log

Alla olevalla komennolla pääsin katsomaan access.logia. 

<img width="579" alt="access log komento" src="https://user-images.githubusercontent.com/122889266/215885315-ba09de48-5aa9-4049-b992-c1b070e371bd.png">

 

<img width="1130" alt="access log" src="https://user-images.githubusercontent.com/122889266/215875887-dbacd8c7-0184-4d5f-8a04-687ebc190b19.png">




/var/log/apache2/error.log

<img width="642" alt="error komento" src="https://user-images.githubusercontent.com/122889266/215875861-e27d3b32-ea1a-4b1e-a1d8-a455f33b1c0b.png">


Ja sain tulostuksen:
<img width="807" alt="error log tulostus" src="https://user-images.githubusercontent.com/122889266/215888222-b26e02db-2ee3-4d1b-8895-dfb1fa138f69.png">

Tulostuksena näkyy ensimmäisenä viikonpäivä, päivämäärä ja kellonaika ja vuosi. 




Onnistunut tapahtuma lokiin 

Kokeilin sammuttaa koneeltani verkkoyhteyden ja testasin näkyisikö se lokissa. 

Sain alla olevan mukaisen kuvan, josta näkee, että verkkoyhteys on katkaistu. 

<img width="809" alt="Yhteys ei toimi" src="https://user-images.githubusercontent.com/122889266/215875716-791dc65c-c125-430d-baea-3e49391034ee.png">

Seuraavassa kuvassa näkyy, että verkkoyhteys toimii taas. 

<img width="811" alt="Yhteys toimii" src="https://user-images.githubusercontent.com/122889266/215861686-2a640d15-01d4-4f71-bb6d-74b18ebc867a.png">

Seuraavaksi yritin aiheuttaa epäonnistuneen tapahtuman lokiin. Yritin antaa väärän salasanan komennolle sudo cat syslog ja katsoin auth.log näkyisikö tapahtuma. Alla testin tulos.

<img width="811" alt="Vaara salasana" src="https://user-images.githubusercontent.com/122889266/215878857-a7c28d7c-e791-49ff-966b-0641484ec5b4.png">























