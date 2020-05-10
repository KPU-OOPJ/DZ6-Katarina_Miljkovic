**Kreirati aplikaciju koji će imati korisnički interfejs kao što je dato na slici i sledeću funkcionalnost:**

-	Javnu klasu Preduzece u paketu pravna_lica koja ima:
-	Privatne atribute PIB (ceo broj), naziv, telefon (ceo broj) i adresa.
-	Odgovarajuće javne get i set metode za ove atribute. Nedozvoljene vrednosti za atribute naziv I adresa su null i prazni Stringovi (""). Pored toga, PIB mora da bude ceo broj veći od nule. U slučaju unosa nedozvoljenih vrednosti baciti izuzetak.
-	Javnu klasu Racun u paketu pravna_lica.prodaja koja ima:
-	Privatni atribut datum koji predstavlja datum izdavanja računa.
-	Privatni atribut iznos (npr. 23.4)
-	Privatni atribut preduzece koji predstavlja objekat klase Preduzece.
-	Odgovarajuće javne get i set metode za sva tri atributa. Datum i preduzeće ne smeju biti null, a iznos mora biti veći od nule. U slučaju unosa nedozvoljenih vrednosti baciti izuzetak.
-	Klasa ProdajaNaVelikoGUI bi trebalo da sadrži privatni atribut racuni koji predstavlja niz objekata klase Racun. Napraviti javni konstruktor koji inicijalizuje ovaj niz na kapacitet 100 elemenata.
-	Kada se pritisne dugme “Obrisi”, preuzimaju se podaci o PIB-u preduzeća iz polja za unos i brišu se svi računi iz niza u kojima preduzeće ima taj PIB. Pored toga, briše se i sadržaj svih polja za unos.
-	Kada se pritisne dugme “Dodaj”, preuzimaju se podaci o preduzeću i iznosu iz polja za unos, pravi se novi račun sa ovim podacima i današnjim datumom i dodaje se u niz na prvo slobodno mesto.
-	Mesto u nizu je slobodno ako je vrednost elementa na tom mestu null. Ako u nizu nema slobodnih mesta, baciti izuzetak.
-	Kada se pritisne dugme “Sacuvaj”, svi podaci o računima (uključujući i podatke o preduzećima) koji su ostvareni prethodnog meseca se upisuju u data fajl "racuni.out" u formatu:
	dan – mesec – godina – PIB – naziv – adresa – telefon – iznos 
-	pri čemu su dan, mesec i godina podaci iz datuma kupovine.

![3](https://scontent.fbeg6-1.fna.fbcdn.net/v/t1.15752-9/96156112_1142612066097716_5060690442241179648_n.png?_nc_cat=103&_nc_sid=b96e70&_nc_eui2=AeG-LkDxtIPsW43zQHiNBzQkCavE_UFcWUkJq8T9QVxZSdK3HWKHScYmqkXLbNr7grE&_nc_ohc=xkrP3K0nAqgAX_0MAiQ&_nc_ht=scontent.fbeg6-1.fna&oh=3025d1878bc2c8570b406d743cbfbab3&oe=5EDD4E9D)
