# Passierschein A38

[![LaTeX](https://img.shields.io/badge/LaTeX-377e7f?logo=latex&logoColor=fff)](https://www.latex-project.org/get/)
[![Static Badge](https://img.shields.io/badge/look-federal-000?logo=europeanunion)](https://de.wikipedia.org/wiki/Schland)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)


Dies ist mein Versuch, den großartigen [Passierschein A38 von blinry](https://blinry.org/passierschein-a38/) in LaTeX im Stil von deutschen Amtsdokumenten nachzubauen.
Die Inhalte der Vorderseite sind mit minimalen Anpassungen wörtlich übernommen.

<img src="passierschein-a38-0.png" width=49% /> <img src="passierschein-a38-1.png" width=49% />


## Blaues Formular

Da der Antrag als Anlage das *Blaue Formular von Schalter I* verlangt, gibt es dieses ebenfalls: nach Rundschreiben B65, in Blaudruck, mit Angaben für die Hafenkommandantur.
Auf der Rückseite liegt das Merkblatt der Hafenkommandantur mit Lageplan, Hafenordnung und abtrennbarer Liegeplatzquittung.

<img src="blaues-formular-0.png" width=49% /> <img src="blaues-formular-1.png" width=49% />


## PDF erzeugen

Mittels LuaLaTeX.
Folgende Hilfsfunktion wird bereitgestellt:

```sh
make passierschein-a38.pdf
make blaues-formular.pdf
# oder
latexmk -cd -f -lualatex -interaction=nonstopmode -synctex=1 --output-directory=__LaTeX-build.nosync -latexoption=--shell-escape passierschein-a38.tex
```


## Lizenz

Wie das Original ist diese Version unter CC BY-SA 4.0 lizensiert.

Für weitere Informationen siehe [LICENSE.md](LICENSE.md).
