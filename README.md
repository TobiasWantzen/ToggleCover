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
This Acrobat Automation Script will only work when placed in one of the Acrobat JavaScript Folders. Execute the following code from the Acrobat JavaScript Console to find the location of the JavaScript folders.

To display the Acrobat JavaScript Console use Ctrl+J on Windows and Command+J on the Mac, does not work properly on newer Mac Books

```javascript
app.getPath("app","javascript");
app.getPath("user");
```
You may have to add a new folder called "JavaScripts" to the user folder manually.

You may place this script file in either one of the folders: Use the "application" folder to install the script for all users, and user the "user" folder to install the script for the user only.

However, the "user" folder is shared by both Acrobat and Reader Placing the file in the user folder will make the menu item availible to both Acrobat and Reader.


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
Das Script funktioniert nur, wenn Sie es in einem der Acrobat-JavaScript-Ordner platzieren.

* Tasten Sie Ctrl-J (Windows) bzw. Cmd-J (Mac), um die Konsole aufzurufen.
* Tippen Sie eine der folgenden Zeilen ein und bestätigen Sie mit Shift-Return oder der Enter-Taste des Nummernfelds:

```javascript
app.getPath("app","javascript");
app.getPath("user");
```
Auf diese Weise erfahren Sie, unter welchem Pfad Sie das Script auf Ihrem Rechner ablegen können. Im user-Ordner müssen Sie evtl. den Ordner „JavaScripts“ noch neu anlegen.

Den »user«-Ordner teilen sich übrigens Acrobat und Acrobat Reader. Dort installierte Skripte stehen ausschließlich dem User selbst zur Verfügung. Bei einer Installation im »application«-Ordner stehen die Skripte allen Usern zur Verfügung.
