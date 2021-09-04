# Notizen Datenspuren

## Google

Der Konzern Google als ein Teil des grossen Konzern Alphabet hat den umfassendsten Zugang zu unseren Geräten. Insbesondere:

- Die Google Suche
- Youtube als die Seite, wo am zweitmeisten gesucht wird
- Google Maps, was schätzungsweise 90% aller Nutzer nutzen
- Google DNS, gemäss einer Studie werden final 30% aller DNS Anfragen der Welt am Ende durch Google aufgelöst
- Android Smartphones als grosse Datenquelle

Google ist so gross, dass man jeden dieser Punkte separat in einer Folge diskutieren könnte. Dabei scheint mir das Smartphone am krassesten zu sein. Auch dort ist ja der Chrome Browser mit drin. 

### Android von Google

### Netzwerk-Scanning

- MAC-Addressen und SSID's sowie Signalstärken. Ist das was alle Geräte halt so tun und dies verlangt auch keine Zustimmung vom Nutzer (crowdsourcing).
- Erfassen Verbindungdaten mit welchem Mobilfunk-Towern man sich verbunden hat (GSM cell tower), das Objekt cell tower ist in der Google Maps API docs definiert, signalStrenth ist eines der Attribute.
- [Rob Braxman](https://yewtu.be/watch?v=4LPDsPvCbCo) behauptet, dass es auf Android für die Wifi-Triangulation einen speziellen Chip gibt, der weiter funktioniert, egal, welches OS man installiert.

Anwendungen:

- Akkurate Bestimmung der Position auch ohne GPS durch Triangulation in Echtzeit
- Positionierung auf der Karte

Im Video wird weiter erklärt, dass die Freigabe des Standorts des Geräts über die Google Location API erfolgt. Das Gerät weiss dank Google und eines der aktiven Lokalisierungverfahrens (WIFI, GPS) wo man sich befindet, und gibt den Standort an die App weiter. WIFI Triangulation wird dazu auch verwendet.

#### Anwendungen

Anhand einer weltweiten Datenbank mit allen Standorten von Routern und SSID's weiss Google, wo man sich befindet. Anhand der Signalstärken kann auch der Standort relativ genau bestimmt werden.

### Telemetrie

- Apps enthalten beim release als apk Google Code, weil sie das hereinbauen müssen
- Apps laufen in einer VM sandboxed auf dem Android
- Zahlungen mussten bis vor kurzen über die Zahlsysteme von Apple und Google abgewickelt werden
- App Nutzungsdaten und Interaktionen


### Firmware

- gibt es custom firmware?