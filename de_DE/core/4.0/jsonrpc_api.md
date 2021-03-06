Hier finden Sie eine Dokumentation zu API-Methoden. Zuerst ist hier
die Spezifikationen (JSON RPC 2.0) :
<http://www.jsonrpc.org/specification>

Der Zugriff auf die API erfolgt über die URL : *URL \ _JEEDOM * / core / api / jeeApi.php

verschiedene
======

Klingeln
----

Pong zurückgeben, Kommunikation mit Jeedom testen

Version
-------

Gibt die Version von Jeedom zurück

Datetime
--------

Gibt die Jeedom-Datumszeit in Mikrosekunden zurück

Konfigurations-API
==========

Config::byKey
-------------

Gibt einen Konfigurationswert zurück.

Einstellungen :

-   String-Schlüssel : Konfigurationswertschlüssel, der zurückgegeben werden soll

-   String Plugin : (optional), Konfigurationswert-Plugin

-   Zeichenfolge Standard : (optional), Wert, der zurückgegeben werden soll, wenn der Schlüssel nicht vorhanden ist
    nicht

Config::speichern
------------

Speichert einen Konfigurationswert

Einstellungen :

-   Zeichenfolgenwert : Wert aufzuzeichnen

-   String-Schlüssel : Konfigurationswertschlüssel zum Speichern

-   String Plugin : (optional), Plugin des Konfigurationswertes zu
    Rekord

JSON-Ereignis-API
==============

Ereignis::Austausch
--------------

Gibt die Liste der Änderungen seit der im Parameter übergebenen Datum / Uhrzeit zurück
(muss in Mikrosekunden sein). Sie haben auch in der Antwort die
Jeedom&#39;s aktuelle Datumszeit (zur Wiederverwendung für die nächste Abfrage)

Einstellungen :

-   int Datetime

JSON Plugin API
===============

Plugin::ListePlugin
------------------

Gibt die Liste alleer Plugins zurück

Einstellungen :

-   int activOnly = 0 (gibt nur die Liste der aktivierten Plugins zurück)

-   int orderByCaterogy = 0 (gibt die Liste der sortierten Plugins zurück
    nach Kategorie)

Objekt-JSON-API
==============

jeeObject::alle
-----------

Gibt die Liste alleer Objekte zurück

jeeObject::voll
------------

Gibt die Liste alleer Objekte zurück, wobei für jedes Objekt allee seine
Ausrüstung und für jede Ausrüstung allee ihre Befehle sowie
Zustände dieser (für Info-Befehle)

jeeObject::vollById
----------------

Gibt ein Objekt mit seiner gesamten Ausrüstung und für jede Ausrüstung zurück
allee seine Befehle sowie ihre Zustände (z
Info-Typ-Befehle)

Einstellungen :

-   int id

jeeObject::BYID
------------

Gibt das angegebene Objekt zurück

Einstellungen:

-   int id

jeeObject::vollById
----------------

Gibt ein Objekt, seine Ausrüstung und für jede Ausrüstung allee seine zurück
Befehle sowie die Zellenzustände (für Typbefehle
info)

jeeObject::speichern
------------

Gibt das angegebene Objekt zurück

Einstellungen:

-   int id (leer, wenn es sich um eine Kreation handelt)

-   Zeichenfolgenname

-   int Vater \ _id = null

-   int isVisible = 0

-   int position

-   Array-Konfiguration

-   Array-Anzeige

JSON-Zusammenfassungs-API
================

Zusammenfassung::insgesamt
---------------

Gibt die insgesamte Zusammenfassung für den im Parameter übergebenen Schlüssel zurück

Einstellungen:

-   String-Schlüssel : (optional), Schlüssel der gewünschten Zusammenfassung, wenn leer, dann Jeedom
    sendet Ihnen die Zusammenfassung alleer Schlüssel

Zusammenfassung::BYID
-------------

Gibt die Zusammenfassung für die Objekt-ID zurück

Einstellungen:

-   int id : Objekt-ID

-   String-Schlüssel : (optional), Schlüssel der gewünschten Zusammenfassung, wenn leer, dann Jeedom
    sendet Ihnen die Zusammenfassung alleer Schlüssel

JSON EqLogic API
================

eqLogic::alle
------------

Gibt die Liste alleer Geräte zurück

eqLogic::vollById
-----------------

Gibt Geräte und ihre Befehle sowie deren Status zurück
(für Info-Bestellungen)

Einstellungen:

-   int id

eqLogic::BYID
-------------

Gibt das angegebene Gerät zurück

Einstellungen:

-   int id

eqLogic::byType
---------------

Gibt allee Geräte zurück, die zum angegebenen Typ gehören (Plugin).

Einstellungen:

-   Zeichenfolgentyp

eqLogic::byObjectId
-------------------

Gibt allee Geräte zurück, die zum angegebenen Objekt gehören

Einstellungen:

-   int object \ _id

eqLogic::byTypeAndId
--------------------

Gibt eine Gerätetabelle gemäß den Parametern zurück. Die Rückkehr
wird vom Formulararray sein (&#39;eqType1&#39; ⇒array (&#39;id&#39;⇒…,&#39; cmds &#39;⇒
Array (….)), &#39;eqType2&#39; ⇒array (&#39;id&#39;⇒…,&#39; cmds &#39;⇒ Array (….))…., id1 ⇒
Array (&#39;id&#39;⇒…,&#39; cmds &#39;⇒ Array (….)), id2 ⇒ Array (&#39; id&#39;⇒…, &#39;cmds&#39; ⇒
Array (....)) ..)

Einstellungen:

-   string \ [\] eqType = Tabelle der erforderlichen Gerätetypen

-   int \ [\] id = Tabelle der gewünschten benutzerdefinierten Geräte-IDs

eqLogic::speichern
-------------

Gibt das registrierte / erstellte Gerät zurück

Einstellungen:

-   int id (leer, wenn es sich um eine Kreation handelt)

-   Zeichenfolge eqType \ _name (Skripttyp, virtuelle Ausrüstung usw.)

-   Zeichenfolgenname

-   Zeichenfolge logische ID = &#39;&#39;

-   int object \ _id = null

-   int eqReal \ _id = null

-   int isVisible = 0

-   int isEnable = 0

-   Array-Konfiguration

-   int timeout

-   Array-Kategorie

JSON Cmd API
============

cmd::alle
--------

Gibt die Liste alleer Befehle zurück

cmd::BYID
---------

Gibt den angegebenen Befehl zurück

Einstellungen:

-   int id

cmd::byEqLogicId
----------------

Gibt allee Bestellungen zurück, die zum angegebenen Gerät gehören

Einstellungen:

-   int eqLogic \ _id

cmd::ExecCmd
------------

Führen Sie den angegebenen Befehl aus

Einstellungen:

-   int id : ID eines Befehls oder ID-Arrays, wenn Sie ausführen möchten
    mehrere Bestellungen gleichzeitig

-   \ [Optionen \] Liste der Befehlsoptionen (abhängig von Typ und
    Befehlssubtyp)

cmd::getStatistique
-------------------

Gibt Statistiken zur Bestellung zurück (funktioniert nur bei
Infos und historische Befehle)

Einstellungen:

-   int id

-   Zeichenfolge startTime : Startdatum der Statistikberechnung

-   Zeichenfolge endTime : Enddatum der Statistikberechnung

cmd::getTendance
----------------

Gibt den Trend für den Befehl zurück (funktioniert nur für die Befehle von
Info und historischer Typ)

Einstellungen:

-   int id

-   Zeichenfolge startTime : Startdatum der Trendberechnung

-   Zeichenfolge endTime : Enddatum der Trendberechnung

cmd::getHistory
---------------

Gibt den Befehlsverlauf zurück (funktioniert nur mit den Befehlen von
Info und historischer Typ)

Einstellungen:

-   int id

-   Zeichenfolge startTime : Startdatum der Geschichte

-   Zeichenfolge endTime : Enddatum der Geschichte

cmd::speichern
---------

Gibt das angegebene Objekt zurück

Einstellungen:

-   int id (leer, wenn es sich um eine Kreation handelt)

-   Zeichenfolgenname

-   Zeichenfolge logische ID

-   Zeichenfolge eqType

-   Zeichenfolgenreihenfolge

-   Zeichenfolgentyp

-   String-Subtyp

-   int eqLogic \ _id

-   int isHistorized = 0

-   string unite = &#39;&#39;

-   Array-Konfiguration

-   Array-Vorlage

-   Array-Anzeige

-   Array HTML

-   int value = null

-   int isVisible = 1

-   Array-Alarm

cmd::Ereignis
-------------------

Ermöglicht das Senden eines Werts an eine Bestellung

Einstellungen:

-   int id

-   Zeichenfolgenwert : Wert

-   Zeichenfolge Datetime : (optional) Wert Datetime

JSON-Szenario-API
=================

Szenario::alle
-------------

Gibt die Liste alleer Szenarien zurück

Szenario::BYID
--------------

Gibt das angegebene Szenario zurück

Einstellungen:

-   int id

Szenario::Export
----------------

Gibt den Export des Szenarios sowie den menschlichen Namen des Szenarios zurück

Einstellungen:

-   int id

Szenario::Import
----------------

Ermöglicht das Importieren eines Szenarios.

Einstellungen:

-   int id : ID des Szenarios, in das Importiert werden soll (leer, wenn erstellt)

-   Zeichenfolge humanName : menschlicher Name des Szenarios (leer bei Erstellung)

-   Array-Import : Szenario (aus dem Feld Exportszenario::Export)

Szenario::Change
---------------------

Ändert den Status des angegebenen Szenarios.

Einstellungen:

-   int id

-   Zeichenfolgenstatus: \ [Run, Stop, aktivieren, deaktivieren \]

JSON-Protokoll-API
============

log::get
--------

Ermöglicht das Wiederherstellen eines Protokolls

Einstellungen:

-   Zeichenfolgenprotokoll : Name des wiederherzustellenden Protokolls

-   String-Start : Zeilennummer, auf der mit dem Lesen begonnen werden soll

-   Zeichenfolge nbLine : Anzahl der wiederherzustellenden Zeilen

log::hinzufügen
--------

Ermöglicht das Schreiben in ein Protokoll

Einstellungen:

-   Zeichenfolgenprotokoll : Name des wiederherzustellenden Protokolls

-   Zeichenfolgentyp : Protokolltyp (Debug, Info, Warnung, Fehler)

-   Zeichenfolge Nachricht : SMS zu schreiben

-   Zeichenfolge logische ID : logische ID der generierten Nachricht


log::Liste
---------

Holen Sie sich die Jeedom-ProtokollListee

Einstellungen:

-   String-Filter : (optional) Filter nach dem Namen der wiederherzustellenden Protokolle

log::leer
----------

Leeren Sie ein Protokoll

Einstellungen:

-   Zeichenfolgenprotokoll : Name des zu leeren Protokolls

log::Entfernen
-----------

Ermöglicht das Löschen eines Protokolls

Einstellungen:

-   Zeichenfolgenprotokoll : Protokollname zum Löschen

JSON-Datenspeicher-API (Variable)
=============================

Datenspeicher::byTypeLinkIdKey
--------------------------

Ruft den Wert einer im Datenspeicher gespeicherten Variablen ab

Einstellungen:

-   Zeichenfolgentyp : Art des gespeicherten Werts (für Szenarien
    es ist Szenario)

-   id linkId : -1 für das insgesamte (Wert für die Standardszenarien,
    oder die Szenario-ID)

-   String-Schlüssel : Wertname

Datenspeicher::speichern
---------------

Speichert den Wert einer Variablen im Datenspeicher

Einstellungen:

-   Zeichenfolgentyp : Art des gespeicherten Werts (für Szenarien
    es ist Szenario)

-   id linkId : -1 für das insgesamte (Wert für die Standardszenarien,
    oder die Szenario-ID)

-   String-Schlüssel : Wertname

-   gemischter Wert : Wert aufzuzeichnen

JSON-Nachrichten-API
================

Nachricht::alle
------------

Gibt die Liste alleer Nachrichten zurück

Nachricht::hinzufügen
--------

Ermöglicht das Schreiben in ein Protokoll

Einstellungen:

-   Zeichenfolgentyp : Protokolltyp (Debug, Info, Warnung, Fehler)

-   Zeichenfolge Nachricht : Nachricht

-   String-Aktion : Aktion

-   Zeichenfolge logische ID : logicalId

Nachricht::EntfernenAll
------------------

Löschen Sie allee Nachrichten

JSON-Interaktions-API
====================

interact::tryToReply
--------------------

Versuchen Sie, eine Anforderung mit einer Interaktion abzugleichen, und führen Sie sie aus
Aktion und reagiert entsprechend

Einstellungen:

-   Abfrage (Anforderungsphrase)

-   int reply \ _cmd = NULL : ID des Befehls, mit dem geantwortet werden soll,
    Wenn nicht angegeben, sendet Jeedom Ihnen die Antwort im JSON

interactQuery::alle
------------------

Gibt die vollständige Liste alleer Interaktionen zurück

JSON-System-API
===============

jeedom::halt
------------

Stoppen Sie Jeedom

jeedom::rebooten
--------------

Starten Sie Jeedom neu

jeedom::ISOK
------------

Lässt Sie wissen, ob der insgesamte Zustand von Jeedom in Ordnung ist

jeedom::Aktualisierung
--------------

Starten wir ein Jeedom-Update

jeedom::Sicherungskopie
--------------

Ermöglicht das Starten eines Backups von Jeedom

jeedom::getUsbMapKlingeln
---------------------

Liste der USB-Anschlüsse und Namen der daran angeschlossenen USB-Sticks

JSON-Plugin-API
===============

Plugin::installeieren
---------------

Installeation / Update eines bestimmten Plugins

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::Entfernen
--------------

Löschen eines bestimmten Plugins

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::dependancyInfo
----------------------

Gibt Informationen zum Status von Plugin-Abhängigkeiten zurück

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::dependancyInstalle
-------------------------

Erzwingen Sie die Installeation von Plugin-Abhängigkeiten

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::deamonInfo
------------------

Gibt Informationen zum Status des Plugin-Daemons zurück

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::deamonStart
-------------------

Zwinge den Dämon zu starten

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::deamonStop
------------------

Dämonenstopp erzwingen

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

Plugin::deamonChangeAutoMode
----------------------------

Ändern Sie den Verwaltungsmodus des Dämons

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)
-   int-Modus : 1 für automatisch, 0 für manuell

JSON-Update-API
===============

Aktualisierung::alle
-----------

Geben Sie die Liste alleer installeierenierten Komponenten, deren Version und die zurück
verwandte Informationen

Aktualisierung::checkUpdate
-------------------

Ermöglicht die Suche nach Updates

Aktualisierung::Aktualisierung
--------------

Ermöglicht das Aktualisieren von Jeedom und alleen Plugins

Aktualisierung::DoUpdate
--------------

Einstellungen:

-   int Plugin \ _id (optional) : Plugin ID
-   Zeichenfolge logische ID (optional) : Plugin Name (logischer Name)

JSON-Netzwerk-API
================

Netzwerk::restartDns
-------------------

Erzwingen Sie den (Neustart) des Jeedom DNS

Netzwerk::stopDns
----------------

Erzwingt das Anhalten des DNS Jeedom

Netzwerk::dnsRun
---------------

Gibt den Jeedom DNS-Status zurück

JSON-API-Beispiele
=================

Hier ist ein Beispiel für die Verwendung der API. Für das folgende Beispiel
Ich benutze [diese Klasse
php] (https://github.com/jeedom/core/blob/stable/core/class/jsonrpcClient.class.php)
Dies vereinfacht die Verwendung der API.

Abrufen der ObjektListee :

``` {.php}
$ jsonrpc = neuer jsonrpcClient (&#39;# URL_JEEDOM # / core / api / jeeApi.php &#39;, # API_KEY #);
if ($ jsonrpc-&gt; sendrequest ( ‚jeeObject::alle &#39;, array ())) {
    print_r ($ jsonrpc-&gt; getResult ());
} Else {
    echo $ jsonrpc-&gt; getError ();
}
```

Ausführung eines Auftrags (mit der Option eines Titels und einer Nachricht)

``` {.php}
$ jsonrpc = neuer jsonrpcClient (&#39;# URL_JEEDOM # / core / api / jeeApi.php &#39;, # API_KEY #);
if ($ jsonrpc-&gt; sendrequest ( ‚cmd::ExecCmd &#39;, Array (&#39; id &#39;=&gt; # cmd_id #,&#39; options &#39;=&gt; array (&#39; title &#39;=&gt;&#39; Cuckoo &#39;,&#39; Nachricht &#39;=&gt;&#39; It works &#39;))) {
    Echo &#39;OK&#39;;
} Else {
    echo $ jsonrpc-&gt; getError ();
}
```

Die API kann natürlich auch in anderen Sprachen verwendet werden (einfach ein Beitrag
auf einer Seite)
