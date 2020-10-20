# CoViD-19---Germany

Ein Dashboard 

## Allgemeine Version


## Freistaat Bayern mit Focus Landshut

### Team

- [Thomas Rogler](https://www.linkedin.com/in/tom-rogler-6405bbb1/)
- [Thomas Massie](https://www.linkedin.com/in/thomasmmassie/)
- [Thomas Hofmann](https://www.linkedin.com/in/thomas-hofmann-a2817646/)

### Eigenschaften

- Schneller Überblick über die wichtigsten Kennzahlen für Bayern und Landshut.
- Leicht verständlich (selbsterklärend).
- Betrachter bekommt ein Gefühl für die Dynamik der Pandemie.
- Vergleiche mit anderen Stadt-/Landkreisen sind möglich; dadurch kann die eigene Lage eingeordnet werden.

### Offene fragen
 
 - **Daten**:
   - Welche Daten wollen wir nutzen und warum? 
     > TMM: Ich bin stark dafür nur Daten abzurufen, welche über eine API abrufbar sind und einen gewissen Mindeststandard aufweisen (z.B. identische Landkreisnamen).
 - **Forecast**: Kann man die Vorhersage vom [Jülich Supercomputing Centre](https://covid19-bayesian.fz-juelich.de/) nutzen? 
   > TMM: So, wie ich das sehe, können wir die Vorhersagen nicht selbst erstellen, no way. Sie bieten die Daten aber auch leider nicht über eine Schnittstelle (API) an.
 - **Ampel**: Die durch die Ampel kodierten Maßnahmen folgen Grenzwerten. Allerdings werden diese evtl. nicht automatisiert angeordnet bzw. wieder aufgehoben. Weiss jemand, wie diese genau wirksam werden?
 
### Aufgaben
 
- [ ] Stadtkreis und Landkreis Landshut zusammenlegen
- [ ] Krankebetten-Daten anpassen, d.h., eindeutige Benennung
- [ ] Ampelfunktion anpassen: Eine Ampel besteht mind. 1 Woche bevor sie wieder heruntergesetzt werden kann. 
  > TMM: **Frage**: Höherstufen passiert sofort? Wäre ja logisch. Allerdings werden die Maßnahmen nicht automatisiert angeordnet, oder (s.o.)?
