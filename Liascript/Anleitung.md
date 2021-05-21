Erste Zeile






/<!--
author:   Your Name

email:    your@mail.org

version:  0.0.1

language: en

narrator: US English Female

comment:  Try to write a short comment about
          your course, multiline is also okay.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

translation: Deutsch  translations/German.md

translation: Français translations/French.md
-->

# LiaScript Grundkurs

erstelle als erstes ein How to (Zielgruppe Lehrende) , wie man mit Liascript startet (in einem Ordner Liascript). Das sollte auf das Tutorial natürlich verweisen, aber ich würde gern, dass man folgendes sehr schnell einsehen kann:
(1) Wie kann ich arbeiten (Browser basiert, mit Github, wie auf dem Desktop und wie sieht der setup da aus (mit links für downloads etc. (alles schon in Liascript)
(2) Wie sieht ein erster Script aus uns was sind die Kernelemente, die ich beachten muss. (Evtl. hier schon mal den kleinen Cheatsheet Ansatz mit zur Bearbeitung in der Gruppe hochladen)
(3) Ab morgen geb ich dir eine Präsi, die dann auch schon mal so mit Inhalten übernommen werden kann :leichtes_lächeln:


Please see the [Docs](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md)
to find out what is possible in [LiaScript](https://liascript.github.io).
s
If you want to use instant help in your Atom IDE, please type **lia** to see all available shortcuts.

## Einrichtung
Voraussetzung um mit LiaScript zu arbeiten ist ein Github Account und die Installation das Programm Atom.

Atom ermöglicht es einen interaktiven Online-Kurs zu erstellen und diesen zu bearbeiten. Mit Github lässt sich der Kurs online speichern und mit anderen Nutzern teilen. Die Links und eine Basis Anleitung für die wesentlichen Funktionen finden sich auf den nächsten Slides.



### Links
[Github Acccount erstellen](https://github.com/join)


[Atom-Download](https://atom.io)

[Basiskurs Youtube](https://www.youtube.com/playlist?list=PL7LrRfaZulhccvNU0Zv6tDAn1OO3D8N8e)

[Basiskurs Github](https://github.com/LiaBooks/LiaScript-Tutorial)


### Installation und Verknüpfung
In Atom müssen folgende Packages installiert werden:

Liascript-preview

liascript-snipptes

Dazu oben links in Atom -> Preferences -> Install nach den beiden packages suchen.

---

Diese [Anleitung](https://www.youtube.com/watch?v=iwMPlVR9M9E&list=PL7LrRfaZulhccvNU0Zv6tDAn1OO3D8N8e&index=16) beschreibt die Einbindung des Githubs Accounts in Atom. Eine Zusammenfassung des Videos folgt außerdem auf den nächsten Slides.

Was ist Github eigentlich? Diesem [Link](https://kinsta.com/de/wissensdatenbank/was-ist-github/) folgen und nachlesen. Lesezeit: 3 Minuten.

---

Die Github Integration ist zum Erstellen eines Kurs nicht zwingend notwendig. [Hier](#7) klicken zum Überspringen der Slides.


### Github Repository erstellen

Für diesen Schritt wird ein Github Account vorrausgesetzt.

Weiter geht es in Atom. Unten rechts findet sich die Schaltfläche Github. Klicken und Log-In wählen. An dieser Steller wird ein Token angefordert, dem entsprechenden Link folgen, Token kopieren und in Atom einsetzten.

Jetzt sollten wir eingeloggt sein und der Button: "Initialize und publish on Gothub" erscheinen.

-> Einen Namen für das Repository festlegen und publish klicken. Auf [Github](https://github.com/) findet sich nun das über Atom erstellte, leere Repository.

### LiaScript Datei auf Github publizieren

In Atom unten rechts neben "Github" klick auf "Git" öffnet den Bereich, in dem Files hochgeladen werden können. Hier sollte unter "Unstaged Changes" das aktuelle File auftauchen, falls nicht: STRG + S (speichern).

Mit Doppellklick lässt sich das File als "Staged Change" einordnen und ist damit ausgewählt zum hochladen.

Abschließend muss eine Commit Message eingeben werden, die entsprechende Änderung beschreibt. Mit Klick auf "commit to main" und "publish" in der Leiste unten rechts wird die Datei hochgeladen und ist nun auf Github einsebar.


Befehle:
Git init
git remote add origin  

(Anleitung alten File)


### Datei erstellen
Um nun mit einem Kurs zu starten muss in Atom mit STRG+N oder oben links in der Leiste ein neues File erstellt werden. Dieses dann sogleich mit der Endung .md speichern.

In die Code Zeile: "liainit" eingeben -> Erstellung des Basiskurs
Kurs anzeigen mit: Kopfleiste: "Packages" -> liascriptpreview -> toggle

Auf der Rechten Seite wird nun der Kurs angezeigt, links der entsprechende Code. Immer wenn gespeichert wird (STRG+S) aktualisiert sich die Vorschau.


## Grundlegende LiaScript Funktionen: Textbearbeitung

Abschnitte festgelegen: Im Code einen oder mehrere Hashtags setzten (-> Roter Text)

Mit Doppellklick auf Code/Vorschau -> Wird Entsprechung im Code/Vorschau angezeigt

Abstände zwischen den Texten in der Preview -> leere Zeile im Code zwischen den Texten

_Kursiv_ schreiben: -> Unterstriche (_) vor und nach dem Text.  

__Fett__ schreiben: -> Zwei Unterstriche (_) vor und nach dem Text.  


___Fett und Kursiv___ schreiben -> Drei Unterstriche (_) vor und nach dem Text

>  Hervorhebung  durch ein (kleiner als)-Zeichen vor dem Code

---

Drei Bindestriche (-) in Folge geben eine Linie. Dafür muss vor und nach der Linie im Code eine Leerzeile stehen

---

### Aufzählungen

Für diese Listen in die Code Zeile "lialist" eingeben und die entsprechende Liste auswählen. Siehe ab Minute 7 in CrashCourse #3

1. Lorem
2. ipsum
3. SumSum

---

*  __Auch hier kann man fett schreiben__

  * Mit Leerzeichen vor dem Code kann man außerdem einrücken

+ Lorem ipsum

---
1. auch Nummerierung ist möglich
  - und einfach
2. Im Code einfach die Zahl mit Punkt dahinter eingeben

Minute 11 mit Links weitermachen


## Beispiele

### A Textquiz

What did the **fish** say when he hit a **concrete wall**?

    [[dam]]

### Multiple Choice

Just add as many points as you wish:

    [[X]] Only the **X** marks the correct point.
    [[ ]] Empty ones are wrong.
    [[X]] ...

### Single Choice

Just add as many points as you wish:

    [( )] ...
    [(X)] <-- Only the **X** is allowed.
    [( )] ...

## Sammlung Fehlermeldungen

### Github Repository erstellen (wahrscheinlich unnötig)



Auf der [Github](https://github.com) Seite befindet sich oben rechts neben dem Namen des gerade eingeloggten Benutzers  ein Plus-Symbol. Jetzt mit Klick auf „New Repository“ ein neues Repository anlegen und einen Namen vergeben. Es öffnet sich ein Fenster, dass einen Link zu eurem Repository bereithält.

Optional: Readme Datei anlegen. Kann genutzt werden, um später Informationen zur Benutzung eurer Software festzuhalten und auf Github anzuzeigen.



### ...


## More

Find out what you can even do more with quizzes:

https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md
