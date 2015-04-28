# Planetarium

![alt text][logo]

[logo]: http://www.unisa.edu.au/Global/ITEE/PLANETARIUM/Planetarium_banner.jpg "Dobrodosli "

## Simulacija kretanja planeta u Suncevom sistemu
### Problem:
######	Simulirati fiktivni ili realni planetarni sistem sa proizvoljnim brojem planeta. Pretpostavka je da se planete krecu oko centralnog tijela po neporemecenim elipticnim putanjama. Kretanje planeta treba da postuje Keplerove zakone.
### Rjesenje:
######	Za ovakve zahtjeve potrebna je pozadinska fizika koju sam implementirao koristeci Three.js biblioteku koja ima odlicnu podrsku za sfernu geometriju koja je u astronomiji i konkretno ovome projektu od krucijalnog znacaja. Iz razloga sto je jedan od dominantnih koordinatnih sistema koji se koristi u astronomiji sferni koordinatni sistem.Velicine i brzinu kretanja plenata sam odabrao tako sto sam skalirao stvarne podatke koje se mogu pronaci na zvanicnom sajtu NASA.

	
	var earthOrbitRadius = 100,
          earthOrbitAngle = 0,
          earthOrbitSpeed = 0.7;
	
######	Svaki od objekata karakterise radijus, ugao i brzina. Defisao sam rotaciju po z osi koja najbolje odgovara polozaju kamere koju sam takodje inijalizovao.

	
	theEarthAndMoon.rotation.z = 23.439281 * Math.PI / 180;
	
###### Rotaciju po osama sam definisam uz pomoc klase koja je definisana u biblioteci Three.js i ciji je jedan od elemenata rotacija. 

######Dakle, nakon postavljanja na scenu svih objekata i definisanja osobina za svaku planetu. Ubacio sam teksture koje se mogu pronaci takodje na NASA sajtu.

######Projekat sam podigao na prostoru koje imam kao student na fakultetskom serveru Alas i mozete da ga pogledate na linku:https://alas.matf.bg.ac.rs/~mi13390/planetarium  

	
![alt text](Screenshot1.png "Logo Title Text 1")
 
![alt text](Screenshot2.png "Logo Title Text 1")
 
![alt text](Screenshot3.png "Logo Title Text 1")

![alt text](Screenshot4.png "Logo Title Text 1")


#### Pitanja, primjedbe i prijedloge mozete slati na moj mail : zeljko94@gmail.com