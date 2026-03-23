# Jupyter Notebooks für Tanenbaum: Computernetzwerke
Jupyter Notebooks für Sachverhalte aus Tanenbaum: Computernetzwerke

Voraussetzungen:

```
pip install numpy matplotlib ipywidgets pandas
```
Optional: 
```
pip install jupyterlab
```

Start:
```
jupyter lab
```
oder
```
jupyter notebook
```
Dann Notebook öffnen und Code ausführen.

## Basisband-Übertragung mit idealem Tiefpass
<img width="953" height="551" alt="grafik" src="https://github.com/user-attachments/assets/1efa4682-166d-4ce1-b200-b062a8853596" />

Simuliert die Übertragung eines digitalen Basisbandsignals über einen Kanal mit begrenzter Bandbreite.

Ziel ist es, anschaulich zu zeigen:
- wie digitale Signale aus Harmonischen aufgebaut sind
- wie Bandbreitenbegrenzung (z. B. durch Kabel) das Signal verzerrt
- wie viele Harmonische für eine „gute“ Übertragung notwendig sind

[Notebook](tanenbaum_bitmuster_bandbegrenzung_ideal.ipynb)
> [!NOTE]
> Notebook wird in Github nicht korrekt angezeigt. Das ist kein Fehler, sondern liegt an den eingebetteten Formeln.

[![Öffnen in Binder](https://mybinder.org/badge_logo.svg)](
https://mybinder.org/v2/gh/DanielBarie/jupyter_tanenbaum/main?labpath=tanenbaum_bitmuster_bandbegrenzung_ideal.ipynb
)

Danach noch auf `Play` in der Menüleiste:  
<img width="615" height="57" alt="grafik" src="https://github.com/user-attachments/assets/7c4c6677-29d8-4787-bb1e-a6582b0bc9a4" />


Dann geht unter dem Code die interaktive Demo auf.

### Features

- Erzeugung eines digitalen Bitmusters (NRZ), Beispiel aus Tanenbaum
- Periodische Wiederholung → definierte Grundfrequenz
- Idealer Tiefpass (Frequenzbereich!)
- Interaktive Steuerung über Anzahl der Harmonischen (Schieberegler)
- Visualisierung:
  - Zeitbereich
  - kontinuierliches Spektrum
  - diskrete Harmonische (Tanenbaum-Stil)

### Bedienung
Slider: „Harmonische“ steuert wie viele Harmonische durchgelassen werden. Entspricht direkt der Kanalbandbreite.

## Interaktive Visualisierung von Basisbandcodes

Dieses Jupyter-Notebook dient zur anschaulichen Visualisierung von Basisbandcodierungen und hilft dabei zu verstehen, wie digitale Bitfolgen in zeitliche Leitungssignale umgesetzt werden.

<img width="967" height="806" alt="grafik" src="https://github.com/user-attachments/assets/7fc7bac7-d5aa-415b-8536-46229d0a1c7b" />

[Notebook](tanenbaum_leitungscodes.ipynb)  
  
[![Öffnen in Binder](https://mybinder.org/badge_logo.svg)](
https://mybinder.org/v2/gh/DanielBarie/jupyter_tanenbaum/main?labpath=tanenbaum_leitungscodes.ipynb
)

[Version mit Darstellung des Spektrums](tanenbaum_leitungscodes_spektrum.ipynb)  
[![Öffnen in Binder](https://mybinder.org/badge_logo.svg)](
https://mybinder.org/v2/gh/DanielBarie/jupyter_tanenbaum/main?labpath=tanenbaum_leitungscodes_spektrum.ipynb
)

### Features

- Interaktive Eingabe beliebiger Bitfolgen
- Visualisierung der folgenden Codierungen:
  - NRZ
  - NRZI
  - Manchester
  - AMI
- Darstellung von:
  - Bitfolge (symbolisch)
  - Signalverlauf (zeitlich)
- Erklärungstabelle pro Bit (inkl. Zustandsübergänge)
- Vergleichsmodus: alle Codierungen gleichzeitig
- Anpassbarer Startpegel für NRZI

### Bedienung

1. Bitfolge in das Eingabefeld eintragen (z. B. `10110010`)
2. gewünschte Codierung auswählen
3. optional:
   - Erklärungstabelle ein-/ausblenden
   - Vergleich aller Codierungen aktivieren
4. der Signalverlauf wird automatisch aktualisiert

### Hinweise

- Es sind nur Bitfolgen aus `0` und `1` erlaubt
- Bei NRZI beeinflusst der Startpegel den Signalverlauf
- Der Vergleichsmodus eignet sich besonders zum Verständnis der Unterschiede zwischen den Codierungen

