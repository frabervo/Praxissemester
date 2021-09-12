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
> Note: Die virtuelle Umgebung ist für die Benutzung von Sphinx. 

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

* Die Veränderung meinem PC in Github posten: Verfahren

(1) git add: Fügt Dateien zum Staging-Bereich hinnzu.
(2) git commit: Kommentiert die Veränderungen 
(3) git push: Verschiebt Dateien in das Online-Verzeichnis

* Synchronisation der Versionenn

  - git commit --> git fetch--> git rebase : `git rebase -i origin/main` --> push

* Git ignore: Welche Dateien oder Verzeichnis müssen nicht geachtet/ ignoriert werden.




## Meine Dokumentation in readthedocs.org hosten

### Was ist readthedocs.org?

READ the Docs ist eine kostenlose Platform zum Hosten von Dokumentationen. Er generiert Dokumentationen, die mit Sphinx geschrieben worden. Die Webseite wurde im JAhr 2010 von Eric Holscher, Bobby Grace und Charles Leifer erstellt. 

### Ein Projekt in readthedocs.org importieren

Um ein Projekt in readthedocs importieren zu können, muss zuerst ein Konto eingerichtet werden. Dann über das Profil auf **my projects** klicken. Da kann ein Projekt importiert werden. 

1. Ein GIthub/ Gitlab Konto verbinden
2. Manuell importieren
3. Infos zu dem Git-Verzeichnis einfügen
    * Name: Praxissemester 
    * Repository-URL: clone über HTTP
    * Repositor-Typ: Git
Dann > next

Für den Aufbau der Dokmentation wird per Default eine Version vorgeschlagen. Sie heißt **lastest**. Es muss überprüft werden, ob das Standard Branch in der erweiterte Einstellung übereinstimmt. 
Administration --> advanced Settings --> Standard-Branch.
Der Link für die Doku: https://praxissemester.readthedocs.io/en/main/

