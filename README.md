# Mainzer Mathe-Akademie 2024: Klimamodellierung und -simulation

Dieses Repository enthält Material zum Kurs
"Klimamodellierung und -simulation"
der [Mainzer Mathe-Akademie 2024](https://freunde.mathematik.uni-mainz.de/mma/).

- Programm: https://freunde.mathematik.uni-mainz.de/files/2024/08/MMA-2024-Programm.pdf
- Übersicht über die Kurse: https://freunde.mathematik.uni-mainz.de/files/2024/08/MMA-Kursbeschreibungen-2024-08-14.pdf


## Installation

Wir verwenden die Programmiersprache [Julia](https://julialang.org).
Um mit dem bereitgestellten Material zu arbeiten, muss Julia heruntergeladen
und installiert werden. Die Links und Anleitung dazu sind auf
https://julialang.org/downloads/
zu finden.
Das Material wurde mit Julia Version 1.10.5 erstellt.

Die einzelnen Bausteine sind von [Pluto.jl](https://github.com/fonsp/Pluto.jl)
Notebooks. Um diese nutzen zu können, muss das Julia-Paket Pluto.jl
installiert werden. Dies kann wie auf der
[offiziellen Pluto.jl Website](https://plutojl.org/)
gemacht werden, um die aktuelle Version von Pluto.jl zu installieren.
Um genau die gleiche Version wie bei der Erstellung des Materials zu verwenden,
können folgende Schritte befolgt werden.

### Mit einem Terminal arbeiten (hauptsächlich Linux oder macOS)

Öffnen Sie ein Terminal (die Konsole) und führen Sie folgenden Code in diesem
Ordner aus:

```bash
julia -e 'import Pkg; Pkg.activate(pwd()); Pkg.instantiate(); import Pluto; Pluto.run()'
```

Danach sollte sich ein Browser-Fenster öffnen, in dem die einzelnen Pluto.jl Notebooks
ausgewählt werden können.

### Windows

Öffnen Sie die Julia REPL - entweder direkt von der Konsole aus oder indem Sie im
Windows Datei Explorer dieses Verzeichnis öffnen und dann in die Adresszeile
"julia" eingeben. Ein Konsolenfenster sollte sich öffnen, in dem Sie folgenden
Code ausführen:

```julia
import Pkg; Pkg.activate(pwd()); Pkg.instantiate(); import Pluto; Pluto.run()
```

Danach sollte sich ein Browser-Fenster öffnen, in dem die einzelnen Pluto.jl Notebooks
ausgewählt werden können.


## Ablauf

- Einführung in die Thematik (Seminarraum)
    - Folien
- Einführung in die Programmierung mit Julia (Seminarraum, Computerraum)
    - Code mit Aufgaben im Notebook `02_Einführung_in_Julia.jl`
    - Statische Darstellung der Aufgaben: https://ranocha.de/2024_MMA_Klima/02_Einführung_in_Julia.html
- Visualisierung einfacher Klimadaten (Computerraum)
    - Code mit Aufgaben im Notebook `03_Visualisierung_einfacher_Klimadaten.jl`
    - Statische Darstellung der Aufgaben: https://ranocha.de/2024_MMA_Klima/03_Visualisierung_einfacher_Klimadaten.html
- Statische 0D Energie-Bilanz-Modelle (Seminarraum)
    - Skript
- Zeitabhängiges 0D Energie-Bilanz-Modell (Seminarraum, Computerraum)
    - Skript
    - Material und Code im Notebook `05_Dynamisches_0D_EBM.jl`
    - Statische Darstellung der Aufgaben: https://ranocha.de/2024_MMA_Klima/05_Dynamisches_0D_EBM.html
- Stochastisches Modell (Seminarraum, Computerraum)
    - Skript
    - Material und Code im Notebook `06_Stochastisches_Modell.jl`
    - Statische Darstellung der Aufgaben: https://ranocha.de/2024_MMA_Klima/06_Stochastisches_Modell.html
- Ausblick auf räumliche Abhängigkeiten (Seminarraum)
    - Skript
    - Material und Code im Notebook `07_Räumliche_Abhängigkeiten.jl`
    - Statische Darstellung der Aufgaben: https://ranocha.de/2024_MMA_Klima/07_Räumliche_Abhängigkeiten.html
