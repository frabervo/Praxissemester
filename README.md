# Praxissemester
Hier werde ich mein Praxissemester organisieren und Kurse zusammen fassen
Dafür habe ein Github reprository erstellt.

## Installtion von der Github 

Mein Github ist mit meiner privaten E-Mail Adresse und meiner Hochschul-E-Mail Adresse.
Ich habe ein Clone von dem Reprository in meinem virtualen Ubuntu erstellt.

## Benutzung der Reprository

Zur Erstellung der Sphinx-Documentation werde ich eine Virtuale Umgebung benutzen.
Diese heißt **virtualenv** und ist über python3.6 installiert worden
* Zum Aktivieren der virtualen Umgebung:

    `source praxissemesterenv/bin/activate` in dem Ordner der Reprository eingeben.\
* Zum Deaktivieren der virtualen Umgebung:

    `deactivate`eingeben

## Sphinx

* Installieren:
    `pip install sphinx` in der Virtuellen Umgebung eingeben. 

* Projekt anfangen:
    `sphinx-quickstart`
    > Name: praxissemester\
    > Autor: Franc Anougon\
    > Project release []: 0.1\
    > Project Language: de

* Die Datei index.rst bearbeiten.\
    Zum Bearbeiten der Datei index.rst muss man die Datei in einem Texteditor öffnen.
    +++ Öffnen: `vim index.rst`
    +++ schließen: 
    +++ Zuerst ** exit** drücken und dann `:wq` eingeben --> zum speichern und zurück auf dem Kommandozeile

* Das Thema (Anzeigeformat) des Webseite ändern:

    1. erste Möglichkeit
    sich ein Thema in der folgende Seite  [theme](https://www.sphinx-doc.org/en/master/usage/theming.html) aussuchen. Dann dieser Name in der Datei conf.py in der Zeile html_theme=... eingeben. 

    2. zweite Möglichkeit 
    ein Thema eines Drittens kann auch verwendet werden. Dafür muss das Thema inportiert werden.
    * Das THema zuerst installieren : `pip install sphinx_rtd_theme`
    * Das Thema importieren: Über die Zeile  html_theme=... folgendes eingeben: import sphinx_rtd_theme 

## Git

* Parameter für meinen Reprository
  ** Name: `git config -global user.name "Franc Anougon"`
  ** E-MAil: `git config -global user.email "bervotigoufack@yahoo.com"`

* Einige Kommandos: 
    + Status abfragen: `git status`
    + Eine Datei/Ordner zum Status staged bringen: `git add dateiname.endung`
    + ein Commit machen: `git commit -m"Nachrit"` oder `git commit` und dannach die Nachricht eingeben.
    + eine Datei oder Ordner vom Zustand **untracked** zu dem zustand **Unmodifed**: git add datei-/Ordnername
    + zum ansehen der Commits: `tig`
    
* Synchronisation der Versionenn
  - git commit --> git fetch-->git rebase : `git rebase -i origin/main` -->push
