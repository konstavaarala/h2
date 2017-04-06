# h2.

## a) Tee tämän kotitehtävän raportti GitHubiin MarkDownilla

### Aloitin käynnistämällä Linuxin livetikulta, jossa käytin versioita ( Xubuntu 16.04 LTS amd64).
Seuraavaksi avasin terminaalin ja annoin komennon $sudo apt-get udate, jotta ohjemistot päivittyvät uusimpiin versioihinsa.
Sitten komento $setxkbmap fi, jotta ääkköset toimivat.
	
### Kirjauduin githubiin tunnuksillani ja loin uuden reporitoryn nimeltä h2, valitsin public ja lisenssiksi GPLv3.0
	
### Sitten asensin gitin komennolla $sudo apt-get -y install git. Kerroin gitille nimen ja sähöpostiosoitteen komennoilla $git config --global user.email "konsta.vaarala@myy.haaga-helia.fi.com" ja #git config --global user.name "Konsta Vaarala".

### Lopuksi kloonataan luotu repository kopioimalla osoite githubista ja syöttämällä komento $git clone https://github.com/konstavaarala/h2.git

### Sitten siirryin luotuun hakemistoon $cd h2/; ja annoin komennot $git add . && git commit; git pull && git push sekä syötin käyttäjätunnuksen sekä salasanan niitä kysyttäessä.

### Loin kansion README, komennolla $nano README, jonne kirjoitin tehtävänannon.

	

## b) Tee puppet-moduli, joka tekee asetukset jollekin komentorivi- tai graafisen käyttöliittymän ohjelmalle.

### Puppetin asennus onnistui komennolla $sudo apt-get -y install puppet

### Seuraavaksi menin puppetin alihakemistoon $cd /etc/puppet/modules, jonne loin oman moduulini $sudo mkdir apacheconf, jonka nimesin apacheconf.
### Menin luotuun kansioon ja loin sen alle kansioit manifests ja templates, komennoilla $sudo mkdir manifests ja $sudo mkdir templates.

### Menin seuraavaksi manifests kansioon $cd manifests, jonne loin init.pp tiedoston komennolla $sudoedit init.pp
### Puppet moduulin pohjaksi otin aikaisemmin käyttämääni Joonan mallia.(https://joonaleppalahti.wordpress.com/2016/10/24/palvelinten-hallinta-harjoitus-1/)

### Lisäsin file osion jonka oli tarkoitus muokata apachen testisivua. Index.html sivun sisältö on täältä (http://terokarvinen.com/2012/short-html5-page) 

### Lopuksi muokkasin init.pp tiedostoa lisäämällä file osion. Ajoin moduulin $sudo puppet apply -e ‘class {apacheconf:}’ ja testisivu vaihtui. Yritin lisätä lopuksi vielä kuvaa lopputilanteesta jossa muuttunut testisivu ja init.pp sisältö näkyisi, mutta en osannut.

## Lähteet 

	http://terokarvinen.com/2013/ssh-server-puppet-module-for-ubuntu-12-04

	http://terokarvinen.com/2012/short-html5-page

	https://guides.github.com/features/mastering-markdown/

	http://terokarvinen.com/2016/publish-your-project-with-github


“Tätä dokumenttia saa kopioida ja muokata GNU General Public License (versio 2 tai uudempi) mukaisesti. http://www.gnu.org/licenses/gpl.html”

“Pohjana Tero Karvinen 2012: Linux kurssi, http://terokarvinen.com”
