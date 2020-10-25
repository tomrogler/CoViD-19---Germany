# CoViD-19---Germany

Ein Dashboard 

## Allgemeine Version


## Freistaat Bayern mit Focus Landshut

### Team

- [Thomas Rogler](https://www.linkedin.com/in/tom-rogler-6405bbb1/)
- [Thomas Massie](https://www.linkedin.com/in/thomasmmassie/)
- [Thomas Hofmann](https://www.linkedin.com/in/thomas-hofmann-a2817646/)

### Rechte (TR)
VORSCHLAG: Die Dashboard Rechte liegen ausschließlich bei TMM. TMM steht es frei bspw. als ASP ein Lizenzmodell für andere Gebietskörperschaften zu realisieren.
TR und TH unterstützen/beraten TMM unentgeltlich bei der Erstellung des Dashboards. Die Stadt Landshut darf das Dashboard kostenfrei nutzen. 

### Ziel (TR)
Maßnahmenakzeptanz durch Kennzahlentransparenz auf gebietskörperschaftabhängigen Dashboard-Startseiten

### Mein Wunsch (TR)
- alle für die Stadt Landshut relevanten Kennzahlen unterschiedlichster Herkunft (Intensivregister, RKI,...) sollen auf einer einzigen Landigpage (personalisierte Dashboard-Startseite) präsentiert und im zeitlichen Verlauf abrufbar gemacht werden.
- auch anderen Gebietskörperschaften (kreisfreie Städte oder Landkreise) soll dieses Werkzeug (URL zu einer personalisierten Dashboard-Startseite) an die Hand gegeben werden

### Eigenschaften
- Schneller Überblick über die wichtigsten Kennzahlen für Bayern und Landshut.
- Leicht verständlich (selbsterklärend).
- BetrachterIn bekommt ein Gefühl für die Dynamik der Pandemie.
- Vergleiche mit anderen Stadt-/Landkreisen sind möglich; dadurch kann die eigene Lage eingeordnet werden.

### Prototyp

Der Prototyp befindet sich auf Tableau Public und kann [hier](https://public.tableau.com/profile/thomas.massie#!/vizhome/CoViD-19---Bayern-Prototype01---Test/Dashboard) aufgerufen werden.

Aktuell sieht dieser so aus:
![Prototyp](https://github.com/thomassie/CoViD-19---Germany/blob/main/04---Screenshots/Bildschirmfoto%202020-10-21%20um%2000.05.37.png)

### Offene fragen
 
- **Daten**:
  - Welche Daten wollen wir nutzen und warum? 
    > *TMM*: Ich bin stark dafür nur Daten abzurufen, welche über eine API abrufbar sind und einen gewissen Mindeststandard aufweisen (z.B. identische Landkreisnamen).
    > *TR*: passt. Bitte beachten: Stand heute muss noch zwischen LK und SK unterschieden werden (kommunale Selbstverwaltung von kreisfreien Städten und Landratsämter).
- **Forecast**: Kann man die Vorhersage vom [Jülich Supercomputing Centre](https://covid19-bayesian.fz-juelich.de/) nutzen? 
   > *TMM*: So, wie ich das sehe, können wir die Vorhersagen nicht selbst erstellen, no way. Sie bieten die Daten aber auch leider nicht über eine Schnittstelle (API) an.
   > *TR*: Leider musste ich feststellen, dass der forecast für Landshut völlig daneben lag. Bitte forecast von der Wunschliste streichen.
- **Ampel**: Die durch die Ampel kodierten Maßnahmen folgen Grenzwerten. Allerdings werden diese evtl. nicht automatisiert angeordnet bzw. wieder aufgehoben. Weiss jemand, wie diese genau wirksam werden?
   > *TR*: Ampel wird schwierig. Hintergrund: es gibt eine gute - aber noch nicht akzeptierte - europäische Ampel mit kombiniertem Indikator. Die staatlich angeordnete bayerische Amel hat mittlerweile eine vierte Farbe bekommen. Einen Algorithmus dafür zu formulieren ist schwierg, da Kommunen auf Antrag die Ampelschaltung ändern lassen können und es zudem eine 6-Tage-Regel gibt. Theoretisch können Kommunen via Allgemeinverfügung auch noch eigene Ampeln gestalten und eigene (zusätzliche) Maßnahmen anordnen. Katastrophe.
- **Aufteilung**: Kann eine Tableau-Landing Page im oberen Teil ein dashboard und im unteren Teil redaktionellen Text beinhalten (vgl. Link München)?
  > *TMM*: Klar! Die Seite kann einrichtet werden wie man möchte. Oder eben verschiedene Seiten...
- **Ansichten**: Kann Tableau responsive design?
  > *TMM*: Logo! Es können diverse Anpassungen (Desktop, iPhone, iPad...) vorgenommen werden.
- **Landing Page**: Mein Wunsch wäre, dass die von uns einzurichtende Subdomain (z.B. corona.landshut.de o.ä), welche die landingpage  darstellt (framelösung).
  > *TMM*: Um das zu verstehen: Das Tableau Dashboard soll in die Website eingebettet werden? Das geht und sollte von den ITlern vor Ort problemlos umgesetzt werden können.
  > *TR*: Entweder Einbettung, frame oder redirect. Kriterium ist hier: das responsive design soll erhalten bleiben
 
### Aufgaben
 
- [ ] Stadtkreis und Landkreis Landshut zusammenlegen.
- [ ] Zeitreihen schnellstmöglich hinzufügen.
- [x] Krankebetten-Daten anpassen, d.h., eindeutige Benennung.
- [ ] Ampelfunktion anpassen: Eine Ampel besteht mind. 1 Woche bevor sie wieder heruntergesetzt werden kann. 
  > *TMM*: Höherstufen passiert sofort? Wäre ja logisch. Allerdings werden die Maßnahmen nicht automatisiert angeordnet, oder (s.o.)?
  > *TR*: "Runterstufen" kann auf Antrag passieren,... schwierig (s.o.)
- [ ] Rechtschreibung und Termini überprüfen/korrigieren
