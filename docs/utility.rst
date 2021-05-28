.. _utility:

==========
Nützliches
==========

--------------------
Individuelle Befehle
--------------------

Individuelle Befehle erlauben dem Bot auf vielseitige Art auf unterschiedliche Dinge zu reagieren.
So kannst du beispielsweise deinen Twitter Account bewerben, deine Discord Einladung anzeigen lassen oder den Bot jemanden pingen lassen!

.. list-table:: Individuelle Befehle
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - command add
     - ``!cb command add "CouchMe" 5 "You have been Couched!"``
     - Erstellt einen Befehl ``CouchMe`` mit einem Cooldown von 5 Sekunden der als Antwort *"You have been Couched!"* ausgibt.
   * - command remove
     - ``!cb command remove "CouchMe"`` 
     - Entfernt einen Befehl, in diesem Fall ``CouchMe``.
   * - command list
     - ``!cb command list``
     - Zeigt die Liste der hinzugefügten Befehle an. Page # ist optional, der Standardwert ist 1.
	 
----------
Moderation
----------

Diese Befehle erlauben grundlegende Moderationsaktionen via CouchBot:

.. list-table:: Moderations Befehle
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - kick
     - ``!cb kick @MattTheDev#0001``
     - Kickt eine Userin vom Server.
   * - ban
     - ``!cb ban @MattTheDev#0001``
     - Verbannt einen User vom Server.
   * - echo
     - ``!cb echo Matt is Great!``
     - Lässt CouchBot den von dir angegebenen Text wiederholen.

----------------------------
Zufällige Benachrichtigungen
----------------------------

Wolltest du schon einmal einen zufälligen Stream in einem Kanal ankündigen? Natürlich wolltest du - und jetzt kannst du das!

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - announce random 
     - ``!cb announce random twitch``
     - Erstellt eine Benachrichtigung für einen zufälligen Stream in dem Kanal, in dem der Befehl ausgeführt wird. (**Nur Admins**)
	    * - dm random
     - ``!cb dm random twitch``
     - Schickt dem User, der den Befehl ausführt, einen zufälligen Stream als DM.

----------------
Sonstige Befehle
----------------

Mit den folgenden Befehlen kannst du verschiedene andere Kleinigkeiten einstellen oder anzeigen lassen.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - info 
     - ``!cb info``
     - Übersicht über verschiedene Statistiken des Bots.
   * - invite
     - ``!cb invite``
     - Schickt dir eine Nachricht mit einem Einladungs-Link für den Bot.
   * - ytidlookup 
     - ``!cb ytidlookup "Channel Name"``
     - Versucht die Kanal ID für YouTube zu ermitteln.
   * - config list 
     - ``!cb config list``
     - Zeigt die Konfiguration des Bots an.
   * - config deleteoffline
     - ``!cb config deleteoffline``
     - Löscht Benachrichtigungen von Streams, die Offline gegangen sind.
   * - config textannouncements
     - ``!cb config textannouncements``
     - Benachrichtigungen werden als Text und nicht als eingebettete Nachrichten angezeigt.
   * - clap 
     - ``!cb clap place your text here``
     - Fügt ein :clap: Emoji zwischen jedes Wort der Nachricht ein.
   * - cookie
     - ``!cb cookie place your text here``
     - Fügt ein :cookie: Emoji zwischen jedes Wort der Nachricht ein.
   * - clone
     - ``!cb clone #ChannelClone All notifications go in here.``
     - Mit diesem Befehl kannst du einen Kanal klonen und die angegebene Nachricht anpinnen.
   * - prefix
     - ``!cb prefix -``
     - Dieser Befehl ändert den Präfix des Bots auf ``-``.

-----------------------
Löschen von Nachrichten
-----------------------

Manchmal kann es vorkommen, dass du sämtliche Nachrichten in einem Kanal, eine bestimmte Anzahl an Nachrichten
oder Nachrichten von bestimmten Usern löschen möchtest um deinen Server effektiv zu moderieren. Das kannst du mit den
folgenden Befehlen bewerkstelligen.

.. Warning:: Du benötigst die **Nachrichten verwalten** Berechtigung, um diesen Befehl ausführen zu können!
			 Einmal ausgeführt können die gelöschten Nachrichten nicht wiederhergestellt werden.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - purge 
     - ``!cb purge``
     - Löscht 100 Nachrichten im aktuellen Kanal.
   * - purge
     - ``!cb purge 25``
     - Löscht 25 Nachrichten im aktuellen Kanal.
   * - purge 
     - ``!cb purge 25 #DiscordChannel``
     - Löscht 25 Nachrichten im Kanal #DiscordChannel. 
   * - purge
     - ``!cb purge 25 #DiscordChannel true``
     - Löscht 25 Nachrichten im Kanal #DiscordChannel inklusive angepinnter Nachrichten.
   * - purge
     - ``!cb purge @MattTheDev``
     - Löscht in den letzten 100 Nachrichten im aktuellen Kanal alle Nachrichten der angegebenen Userin.
   * - purge
     - ``!cb purge @MattTheDev true``
     - Löscht in den letzten 100 Nachrichten im aktuellen Kanal alle Nachrichten inklusive angepinnter Nachrichten des angegebenen Users.
   * - purge
     - ``!cb purge @MattTheDev #DiscordChannel``
     - Löscht in den letzten 100 Nachrichten im Kanal #DiscordChannel alle Nachrichten des angegebenen Users.
   * - purge
     - ``!cb purge @MattTheDev #DiscordChannel true``
     - Löscht in den letzten 100 Nachrichten im Kanal #DiscordChannel alle Nachrichten inklusive angepinnter Nachrichten der angegebenen Userin.

.. Warning:: Die folgenden Befehle haben keine Bestätigung und werden nach Aufruf ausgeführt.

.. list-table:: Löschen von Content Creators
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - creators purge 
     - ``!cb creators purge``
     - Entfernt die Benachrichtigungen für alle manuell hinzugefügten Content Creators.
   * - creators purge 
     - ``!cb creators purge twitch``
     - Entfernt die Benachrichtigungen für alle manuell hinzugefügten Twitch Content Creators.
