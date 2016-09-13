# LaTeX-Vorlage für Projekt- und Bachelorarbeiten  

## Grundsätzliches
* LaTeX-Vorlage für Projekt- und Bachelorarbeiten an der DHBW Mannheim (Wirtschaftsinformatik / Software Engineering).
Die Vorlage ist *lediglich als Muster anzusehen!* Konkrete formale Ausgestaltungen, Zitationsstil usw. sollten *unbedingt* mit dem
wissenschaftlichen Betreuer abgestimmt werden!
* **Bitte beschäftigen Sie sich mit LaTeX, da diese Vorlage ein gewisses LaTeX-Verständnis voraussetzt!**


## Installationsanweisungen

### Voraussetzungen

Sie benötigen zunächst eine laufende LaTeX-Installation.

* Windows-User: [MikTex](http://www.miktex.org)
* Mac-User: [MacTex](http://www.tug.org/mactex/index.html)
* Linux-User: [TexLive](http://www.tug.org/texlive/) (meist bei den Distributionen dabei)

Neben einer laufenden LaTeX-Installation benötigen Sie weiterhin noch einen Editor.
Vorschläge für LaTeX-Editoren:

* [TexStudio](http://www.texstudio.org) (Plattformübergreifend)
* [TexShop](http://pages.uoregon.edu/koch/texshop/) (Mac)

### Installation der eigentlichen Vorlage

Bitte laden Sie die Vorlage entweder als ZIP-Paket oder per `git clone`-Befehl auf Ihren Rechner. Im Falle eines ZIP-Downloads müssen Sie die ZIP-Datei entpacken. Die Vorlage selbst ist weitestgehend Standard-LaTeX und es existieren lediglich zwei vorlagenspezifische Befehle, die _nicht_ im LaTeX-Standard enthalten sind [(siehe unten)](#markdown-header-vorlagenspezifische-befehle). In der Vorlage finden Sie viele Kommentare als auch ein Anleitungskapitel, welches die Arbeitsweise
der Vorlage beschreibt, daher an dieser Stelle der Verweis auf die Vorlage selbst. Ebenfalls in der Vorlage enthalten sind
Beispiele für das Zitieren von Quellen (Artikel, Buch, Online-Quelle, siehe Datei `bibliography.bib`).

**Wichtig:** Anstelle des älteren BibTeX verwendet die Vorlage für die Erstellung der Bibliographie
die neueren Pakete BibLaTeX und Biber. Je nach von Ihnen verwendetem Editor müssen Sie in den Editor-Einstellungen
entsprechende Änderungen vornehmen!

## Aufbau der Vorlage
Die Datei `master.tex` ist die Hauptdatei der Vorlage, die übersetzt werden kann. Von hier werden auch die anderen
Dateien entsprechend eingezogen. Bitte schauen Sie sich die Kommentare in der Datei an, um ggf. nicht relevante
Verzeichnisse (z.B. ein Algorithmenverzeichnis) auszublenden.

Die Datei `config.tex` zieht relevate Pakete ein und konfiguriert diese. Hier können faktisch alle Eigenschaften der Vorlage
(Zitierstil, Layout etc.) verändert werden. Beachten Sie auch hier die Kommentare in der Datei selbst sowie die im Internet
auf [CTAN](http://www.ctan.org) erhältlichen Dokumentationen der verwendeten Pakete.


## Vorlagenspezifische Befehle
- `\AutorDerArbeit{Max Mustermann}` setzt den Autor der Arbeit entsprechend auf *Max Mustermann*,
- `\TitelDerArbeit{Ein Testtitel}`setzt den Titel der Arbeit auf *Ein Testtiitel*

Deckblatt, Kurzfassung und Selbständigkeitserklärung werden mit diesen Informationen
befüllt und sollten an der entsprechenden Stelle in der Datei `master.tex`
gesetzt werden.
