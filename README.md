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


## Working from a terminal (e.g., Linux or macOS)

Open a terminal and run

```bash
julia -e 'import Pkg; Pkg.activate("."); Pkg.instantiate(); import Pluto; Pluto.run()'
```

in this directory. Then, open the Pluto notebook `online_stats.jl`.


## Windows

Open the Julia REPL in this directory, e.g., by navigating to this directory
in the Windows File Explorer and typing "julia" the address bar. A console
window should open. There, execute

```julia
import Pkg; Pkg.activate("."); Pkg.instantiate(); import Pluto; Pluto.run()
```

in the Julia REPL. Then, open the Pluto notebook `online_stats.jl`.

