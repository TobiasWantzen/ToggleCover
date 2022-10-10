# ToggleCover [EN]
Acrobat script for Acrobat Pro or Acrobat Reader to toggle easily between different views, with or without the cover page, in the frontmost PDF.

Visit the corresponding blog post here (available only in German): https://wantzen.com/blog/arcobat-script-togglecover-umschalten-der-seitenanzeige/

## How to use
The script can be integrated into the quick toolbar, called up via the additional tools, or accessed via the "view" menu: "Two page view: Toggle Cover Page View".

## Logic
The script switches the page view according to the following logic:

|Active page view|Script changes view to|
|:---|:---|
|Two Page View *and* Show Cover Page|Two Page View *and* No Cover Page|
|Two Page View *and* No Cover Page|Two Page View *and* Show Cover Page|
|All other views|Two Page View *and* Show Cover Page|

## General installation instructions
This Acrobat script will only work when placed in one of the Acrobat JavaScript folders.

*For Windows:*

* Place the script file "ToggleCover.js" in this folder (or the same folder in the full version):\
  `C:\Program Files (x86)\Adobe\Acrobat Reader DC\Reader\Javascripts\`
* Restart Acrobat.

*For Mac:*

* In Finder, go to your Acrobat.app in the Applications folder.
* Right-click on the Acrobat.app and select "View Package Contents" to view the inside of the app package.
* Inside the app navigate to this directory:\
  `Acrobat.app/Contents/Resources/JavaScripts/`
* Place the script file "ToggleCover.js" there.
* Restart Acrobat.

If this does not work, you can find out the directory on your computer as follows:

* Key Ctrl+J (Windows) or Cmd+J (Mac) to bring up the console.
* Type *one* of the following lines and confirm with Ctrl+Return (Windows) or Command+Return (Mac) or the Enter key of the number pad:

```javascript
app.getPath("app","javascript");
app.getPath("user");
```
This way you will know under which path you can place the script on your computer. In the user folder you may have to create the folder "JavaScripts".

The "user" folder is shared by Acrobat and Acrobat Reader. Scripts installed there are only available to the user. If they are installed in the "application" folder, the scripts are available to all users.



# ToggleCover [DE]
Ein Acrobat-Skript für Acrobat Pro oder den Acrobat Reader, mit dem Sie einfach zwischen verschiedenen Ansichten – mit und ohne Cover – im aktiven PDF wechseln können.

Besuchen Sie den dazugehörenden Blog-Beitrag: https://wantzen.com/blog/arcobat-script-togglecover-umschalten-der-seitenanzeige/

## Anwendung
Das Script lässt sich in die Schnellwerkzeug-Leiste integrieren, über die Zusatzwerkzeuge aufrufen oder über das "Anzeige"-Menü ansteuern: "Zweiseitenansicht: Deckblatt umschalten".

## Umschaltlogik
Das Script schaltet die Seitenansicht nach folgender Logik um:

|Aktive Seitenansicht|Skript wechselt die Ansicht zur|
|:---|:---|
|Zweiseitenansicht mit Deckblatt|Zweiseitenansicht ohne Deckblatt|
|Zweiseitenansicht ohne Deckblatt|Einseitenansicht|
|Alle anderen Ansichten|Zweiseitenansicht mit Deckblatt|

## Installationsanleitung
Das Script funktioniert nur, wenn Sie es in einem der Acrobat-JavaScript-Ordner platzieren:

*Für Windows:*

* Legen Sie die Scriptdatei "ToggleCover.js" in diesen (bzw. in der Vollversion gleichlautenden) Ordner:\
  `C:\Programme (x86)\Adobe\Acrobat Reader DC\Reader\Javascripts\`
* Starten Sie Acrobat neu.

*Für Mac:*

* Gehen Sie im Finder zu Ihrer Acrobat.app im Programme-Ordner.
* Klicken Sie mit der rechten Maustaste auf die Acrobat.app und wählen Sie »Paketinhalt anzeigen«, um das Innere der Applikation anzuzeigen.
* Navigieren Sie innerhalb der App in das Verzeichnis:\
  `Acrobat.app/Contents/Resources/JavaScripts/`
* Platzieren Sie die Scriptdatei "ToggleCover.js" dort
* Starten Sie Acrobat neu.

Sollte das nicht funktionieren, können Sie das Verzeichnis auf Ihrem Rechner wie folgt ermitteln:

* Tasten Sie Ctrl+J (Windows) bzw. Cmd+J (Mac), um die Konsole aufzurufen.
* Tippen Sie *eine* der folgenden Zeilen ein und bestätigen Sie mit Strg+Return (Windows) bzw. Befehl+Return (Mac) oder der Enter-Taste des Nummernfelds:

```javascript
app.getPath("app","javascript");
app.getPath("user");
```
Auf diese Weise erfahren Sie, unter welchem Pfad Sie das Script auf Ihrem Rechner ablegen können. Im user-Ordner müssen Sie evtl. den Ordner „JavaScripts“ noch neu anlegen.

Den »user«-Ordner teilen sich übrigens Acrobat und Acrobat Reader. Dort installierte Scripte stehen ausschließlich dem User selbst zur Verfügung. Bei einer Installation im »application«-Ordner stehen die Scripte allen Usern zur Verfügung.
