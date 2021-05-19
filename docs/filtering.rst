.. _filtering:

======
Filter
======

.. note:: All diese Befehle sind ein/aus Schalter. Wenn du etwas von der Liste entfernen möchtest führe einfach den entsprechenden Befehl ein zweites Mal aus.

**CouchBot** ermöglicht das Filtern von spezifischen Spielen oder Stream Titeln.
Dadurch werden von allen hinzugefügten Content Creators nur Streams angekündigt, die ein Spiel oder einen Titel beinhalten, der auf der Filterliste steht.
Würde beispielsweise jemand Destiny 2 spielen würden diese Streams im folgenden Beispiel nicht angekündigt werden.

.. list-table:: Filter Befehle
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - filter game
     - ``!cb filter game twitch "World of*"``
     - Erstellt auf Twitch einen **Spiele Filter** für alle Spiele die mit "World of" beginnen.
   * - filter title
     - ``!cb filter title twitch "World of*"``
     - Erstellt auf Twitch einen **Stream Titel Filter** für alle Titel die mit "World of" beginnen.
   * - filter list
     - ``!cb filter list``
     - Zeigt eine Liste aller aktuell aktiven Filter an.
	 
