# Local Library
## Voorwoord
Ik had toch best wat moeite met Django. Het is me echter wel gelukt om deze hele simpele app te maken conform de eisen. Het originele idee om een video calling app te maken heb ik maar geschrapt, sinds ik hier geen degelijke informatie over kon vinden online wat nog up-to-date was voor nieuwere Django versies.

## Features
 - Create, Read, Update, Delete Authors, Books, and Book Instances as Admin
 - View how many times you visited the site as user
 - View which books are aviable

## Uitleg
Deze applicatie stelt een bibliotheek voor. Hier kun je als admin nieuwe boeken toevoegen, en nieuwe book instances aanmaken. Een boek instance stelt een 'fysiek' boek voor, wat een status kan hebben zoals 'beschikbaar', 'uitgeleend' etc.

Een gebruiker van de website kan de autheurs zien, en ook alle boeken. Elk boek heeft een detail view waar meer info kan worden bekeken.

## Instructies
- Een nieuwe python virtual env maken (optioneel maar aangeraden)
- Met pip requirements.txt installeren `pip3 install -r requirements.txt`
- Als het goed is hoef je geen migrations te maken sinds je het bijgevoegde `db.sqlite3` bestand hebt. Anders moet je wel even `python3 manage.py makemigrations` en daarna `python3 manage.py migrate` doen. Daarna zou je `python3 manage.py createsuperuser` moeten doen om een superuser te maken.
- `python manage.py runserver`
- Ga naar http://127.0.0.1:8000/admin, log in met username: `floris`, password: `codeblauw`. Als je zelf een superuser hebt gemaakt, kun je natuurlijk met die gegevens inloggen.
- Voeg wat boeken toe, je kunt dan ook meteen Authors en Genres toevoegen.
- Voeg wat book instances toe
- Ga naar http://127.0.0.1:8000/ of http://127.0.0.1:8000/catalog om de voorkant te zien.

## Reflectie
De manier van werken met Django vond ik erg geopinieerd. Wat ik daar mee bedoel is dat het een grote investering is om comfortabel met de werkwijze te worden, terwijl deze vrijwel uniek aan Django is en je er dus niet veel aan hebt buiten Django. Dit had ook geen goede gevolgen voor mijn motivatie. Ik vind het erg jammer dat ik hierdoor een project moet opleveren wat in mijn ogen erg onder mijn standards ligt. Toch probeer ik te accepteren dat ik niet elke manier van werken geweldig kan vinden, en ik blij mag zijn dat mijn app aan de project eisen voldoet.