# Armaturenbrett
**Home → Armaturenbrett**

<small>[Raccourcis clavier/souris](shortcuts.md)</small>

Auf einer der Hauptseiten von Jeedom wird ein Bericht über Ihre gesamte Hausautomation angezeigt.
Dieser Bericht wird (im Gegensatz zu Ansichten und Designs) von Jeedom selbst erstellt und enthält alle sichtbaren Objekte und deren Ausrüstung.

> **Spitze**
>
> Die Anzeigereihenfolge der Objekte im Armaturenbrett ist die in **Analyse → Zusammenfassung der Hausautomation**. Sie können diese Reihenfolge ändern, indem Sie auf diese Seite ziehen und dort ablegen.

Damit Geräte im Armaturenbrett angezeigt werden, muss dies der Fall sein :
- Sei aktiv.
- Sei sichtbar.
- Haben Sie als übergeordnetes Objekt ein Objekt im Armaturenbrett sichtbar.

Beim ersten Erscheinen der Ausrüstung im Armaturenbrett versucht Jeedom, die Größe der Kachel korrekt anzupassen, um alle Befehle und ihre Widgets anzuzeigen.
Um ein ausgewogenes Armaturenbrett zu erhalten, können Sie mit dem Stift oben rechts in der Suchleiste in den Bearbeitungsmodus wechseln, um die Größe der Gerätekacheln zu ändern und / oder sie neu zu ordnen.

Wenn Sie mit der Maus über eine Bestellung fahren, wird unten links auf der Kachel eine farbige Markierung angezeigt:
- Blau für eine Info-Bestellung. Wenn es protokolliert ist, öffnet ein Klick darauf das Protokollfenster.
- Orange für einen Aktionsbefehl. Ein Klick löst die Aktion aus.

Außerdem können Sie auf den Titel der Kachel (den Namen des Geräts) klicken, um die Konfigurationsseite dieses Geräts direkt zu öffnen.

> **Spitze**
>
> Über das Menü können Sie direkt zu einem einzelnen Objekt in Ihrer Hausautomation wechseln **Home → Armaturenbrett → Objektname**.
> Auf diese Weise haben Sie nur die Ausrüstung, die Sie interessiert, und können die Seite schneller laden.

- Oben links befindet sich ein kleines Symbol zum Ein- und Ausblenden des Objektbaums.
- Mit dem zweiten Symbol links können nur die Informationen der Zusammenfassungen der Objekte angezeigt werden.
- In der Mitte können Sie in einem Suchfeld nach Geräten nach Name, Kategorie, Plugin, Tag usw. suchen..
- Auf der rechten Seite können Sie über eine Schaltfläche in den Bearbeitungsmodus wechseln, die Reihenfolge der Kacheln ändern (geklickt - im Widget abgelegt) oder ihre Größe ändern. Sie können auch in einer Kachel die Reihenfolge der Bestellungen neu anordnen.
- Durch Klicken auf eine Objektzusammenfassung filtern Sie, um nur die Geräte anzuzeigen, die sich auf dieses Objekt beziehen und die sich auf diese Objektzusammenfassung beziehen.
- Ein Klick auf einen Auftrag vom Informationstyp zeigt den Verlauf des Auftrags an (falls er historisch ist)..

> **Spitze**
>
> In Ihrem Profil können Sie Jeedom so konfigurieren, dass der Baum der Objekte und / oder die Szenarien standardmäßig sichtbar sind, wenn Sie im Armaturenbrett ankommen.

> **Spitze**
>
> Wenn Sie auf Mobilgeräten einen Befehl vom Typ &quot;Info&quot; drücken, wird ein Menü angezeigt, in dem Sie entweder den Verlauf der Bestellung anzeigen oder eine Warnung darauf setzen können, damit Jeedom Sie (einmal) benachrichtigt, sobald dass der Wert einen bestimmten Schwellenwert überschreitet.


## Bearbeitungsmodus

Im Bearbeitungsmodus (* der Stift oben rechts *) können Sie die Größe der Kacheln und ihre Anordnung im Armaturenbrett ändern.

Sie können auch das interne Layout der Steuerelemente auf der Kachel bearbeiten :

- Ordnen Sie sie entweder durch Ziehen und Ablegen neu an.
- Entweder durch Klicken mit der rechten Maustaste auf das Widget. Sie greifen dann zu :
    - **Erweiterte Konfiguration** : Ermöglicht den Zugriff auf die erweiterte Konfiguration des Befehls.
    - **Standard** : Standardlayout, alles ist automatisch mit nur der Möglichkeit, die Reihenfolge der Bestellungen neu zu ordnen.
    - **Tabelle** : ermöglicht das Einfügen der Befehle in eine Tabelle : Spalten und Zeilen werden durch Klicken mit der rechten Maustaste hinzugefügt und gelöscht. Verschieben Sie dann einfach die Befehle in die gewünschten Felder. Sie können mehrere Bestellungen pro Box aufgeben
    - **Spalte hinzufügen** : Fügen Sie der Tabelle eine Spalte hinzu (nur verfügbar, wenn Sie sich im Tabellenlayout befinden).
    - **Zeile hinzufügen** : Fügen Sie der Tabelle eine Zeile hinzu (nur verfügbar, wenn Sie sich im Tabellenlayout befinden).
    - **Säule entfernen** : Entfernen Sie eine Spalte aus der Tabelle (nur verfügbar, wenn Sie sich im Tabellenlayout befinden).
    - **Zeile löschen** : Löschen Sie eine Zeile in der Tabelle (nur verfügbar, wenn Sie sich im Tabellenlayout befinden).

Rechts von jedem Objekt können Sie ein Symbol verwenden :

- klicken : Alle Kacheln dieses Objekts nehmen eine Höhe an, die der höchsten Kachel entspricht.
- Strg Klicken Sie auf : Alle Kacheln dieses Objekts nehmen eine Höhe an, die der niedrigsten Kachel entspricht.

## Jeedom Menüleiste

> **Spitze**
>
> - Klicken Sie auf die Uhr (Menüleiste) : Öffnen Sie die Timeline.
> - Klicken Sie auf den Namen des Jeedom (Menüleiste) : Öffnet Einstellungen → System → Konfiguration.
> - Klicken Sie auf ? (Menüleiste) : Öffnet die Hilfe auf der aktuellen Seite.
> - Flucht auf ein Forschungsfeld : Leeren Sie das Suchfeld und brechen Sie es ab.
