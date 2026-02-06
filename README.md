**Viikkotehtävä 4 - Navigointi Jetpack Composessa**

**Navigointi Jetpack Composessa**

Navigointi Jetpack Composessa tarkoittaa näkymien (Composable-funktioiden) välistä siirtymistä yhden aktiviteetin sisällä. Sovellus käyttää Single-Activity-arkkitehtuuria ja Navigation Compose -kirjastoa.

NavController vastaa navigoinnin ohjaamisesta ja reittien vaihtamisesta.
NavHost määrittelee sovelluksen navigaatiorakenteen ja kertoo, mikä näkymä näytetään milläkin reitillä.

**Sovelluksen navigaatiorakenne**

Sovelluksessa on kaksi pääruutua:

**HomeScreen** (tehtävälista)

**CalendarScreen** (kalenterinäkymä)

Käyttäjä voi siirtyä HomeScreeniltä CalendarScreenille ja takaisin NavControllerin avulla. Back-nappi toimii sekä järjestelmän että sovelluksen oman navigaation kautta.

**MVVM ja jaettu ViewModel**

Sovellus käyttää MVVM-arkkitehtuuria.
Sama TaskViewModel jaetaan HomeScreenin ja CalendarScreenin välillä, joten ViewModel ei katoa navigoinnin aikana. Molemmat ruudut lukevat ja muokkaavat samaa tilaa, ja muutokset näkyvät heti molemmissa näkymissä.

**CalendarScreen**

CalendarScreen näyttää tehtävät kalenterimaisessa näkymässä. Tehtävät ryhmitellään niiden päivämäärän (dueDay) mukaan, ja jokaisen päivän alla näkyvät siihen kuuluvat tehtävät listana.

**Tekijä:** Kasperi Mustonen

