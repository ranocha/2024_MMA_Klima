# Mainzer Mathe-Akademie 2024: Klimamodellierung und -simulation

[![License: MIT](https://img.shields.io/badge/License-MIT-success.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13766641.svg)](https://doi.org/10.5281/zenodo.13766641)

Dieses Repository enthält Material zum Kurs
"Klimamodellierung und -simulation"
der [Mainzer Mathe-Akademie 2024](https://freunde.mathematik.uni-mainz.de/mma/).

- Programm: https://freunde.mathematik.uni-mainz.de/files/2024/08/MMA-2024-Programm.pdf
- Übersicht über die Kurse: https://freunde.mathematik.uni-mainz.de/files/2024/08/MMA-Kursbeschreibungen-2024-08-14.pdf

> Der Klimawandel mit seinen Auswirkungen ist ein Thema, zu dem
> viele Menschen eine starke Meinung haben. Um sachlich darüber
> diskutieren zu können, sollte man allerdings auch die wissenschaftliche
> Seite verstehen, in der Klimamodelle eine wesentliche Rolle spielen.
> Wir werden einen Blick unter die Haube solcher Klimamodelle werfen.
> Dazu betrachten wir zunächst die notwendigen Grundlagen der Analysis
> (Ableitungen) und nutzen diese für eine mathematisch-physikalische
> Modellierung des Klimas. Da die entstehenden Gleichungen sehr komplex
> sind, benötigen wir numerische Verfahren, um das Lösungsverhalten zu
> verstehen. Glücklicherweise können uns Computer die eigentliche
> Rechenarbeit abnehmen, sodass wir "nur noch etwas programmieren
> müssen".


## Installation

Wir verwenden die Programmiersprache [Julia](https://julialang.org).
Um mit dem bereitgestellten Material zu arbeiten, muss Julia heruntergeladen
und installiert werden. Die Links und Anleitung dazu sind auf
https://julialang.org/downloads/
zu finden.
Das Material wurde mit Julia Version 1.10.5 erstellt.

Auf den Computern der Universität Mainz ist Julia unter Linux schon installiert.
Wenn Sie lieber mit Windows arbeiten möchten, müssen Sie Julia gegebenenfalls
selbst installieren. Dazu müssen Sie Julia als
[ZDV-App installieren](https://www.zdv.uni-mainz.de/zdvapps-software-am-arbeitsplatz/).
Die Installation unter Linux ist aber besser getestet und im Zweifelsfall zu
bevorzugen.

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
`julia` eingeben. Ein Konsolenfenster sollte sich öffnen, in dem Sie folgenden
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


## Quellen

Detaillierte Quellenangaben finden Sie in den zugehörigen Notizen, die in der
Veranstaltung verteilt werden.
Darüber hinaus wurde dieser Kurs von Material der Lehrveranstaltung
*An introduction to Climate Modeling* im Sommersemester 2023 an
der Universität zu Köln inspiriert, die von Gregor Gassner und
Andrés Rueda-Ramírez geleitet wurde und durch Beiträge von Daniel Bach,
Sophia Schmickler, Erik Faulhaber und Luca Sommer unterstützt wurde.

Ein einfaches Klimamodell, das auf den hier behandelten Themen (ohne die
stochastischen Einflüsse) basiert und zusätzlich räumliche Abhängigkeiten
in Form partieller Differentalgleichungen modelliert ist in dem Prototyp
[Klimakoffer.jl](https://github.com/klimakoffer/Klimakoffer.jl) implementiert.
