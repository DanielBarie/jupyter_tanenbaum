# Jupyter Notebooks für Tanenbaum: Computernetzwerke
Jupyter Notebooks für Sachverhalte aus Tanenbaum: Computernetzwerke

Voraussetzungen:

```
pip install numpy matplotlib ipywidgets
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


