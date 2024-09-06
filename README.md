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
- Einführung in die Programmierung mit Julia:
    - Code mit Aufgaben im Notebook `02_Einführung_in_Julia.jl`
- Visualisierung einfacher Klimadaten
