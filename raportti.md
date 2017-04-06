# h2.

## a) Tee tämän kotitehtävän raportti GitHubiin MarkDownilla

	Aloitin käynnistämällä Linuxin livetikulta, jossa käytin versioita ( Xubuntu 16.04 LTS amd64). Seuraavaksi avasin terminaalin ja annoin komennon $sudo apt-get udate, jotta ohjemistot päivittyvät uusimpiin versioihinsa. Sitten komento $setxkbmap fi, jotta ääkköset toimivat.
	
	Kirjauduin githubiin tunnuksillani ja loin uuden reporitoryn nimeltä h2, valitsin public ja lisenssiksi GPLv3.0
	
	Sitten asensin gitin komennolla $sudo apt-get -y install git. Kerroin gitille nimen ja sähöpostiosoitteen komennoilla $git config --global user.email "konsta.vaarala@myy.haaga-helia.fi.com" ja #git config --global user.name "Konsta Vaarala".

	Lopuksi kloonataan luotu repository kopioimalla osoite githubista ja syöttämällä komento $git clone https://github.com/konstavaarala/h2.git

	Sitten siirryin luotuun hakemistoon $cd h2/; ja annoin komennot $git add . && git commit; git pull && git push sekä syötin käyttäjätunnuksen sekä salasanan niitä kysyttäessä.

	Loin kansion README, komennolla $nano README, jonne kirjoitin tehtävänannon.

	

## b) Tee puppet-moduli, joka tekee asetukset jollekin komentorivi- tai graafisen käyttöliittymän ohjelmalle.

