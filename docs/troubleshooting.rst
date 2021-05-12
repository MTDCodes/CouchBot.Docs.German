.. _troubleshooting:

==============
Fehlerbehebung
==============

Du kannst dem CouchBot Support Server unter diesem Link beitreten --> https://discord.couch.bot/

------------------------
Benötigte Berechtigungen
------------------------

Wenn **CouchBot** deinem Server beitritt sollte ein Fenster auftauchen, in dem er alle notwendigen Berechtigungen anfordert.
Um sicher zu gehen dass **CouchBot** vollständig auf deinem Server funktioniert stelle bitte sicher, dass seine Server Rolle die folgenden Berechtigungen zugewiesen hat:

- Rollen verwalten (für Live Discovery / Rollen Zuweisungen)
- Kanäle ansehen (für ALLE Funktionen)
- Nachrichten senden (für ALLE Funktionen)
- Nachrichten verwalten (für DeleteOffline Funktionen)
- Links einbetten (für ALLE Funktionen)
- Nachrichtenverlauf anzeigen (für ALLE Funktionen)
- Erwähne @everyone, @here und "Alle Rollen" (für Ping Funktionen)

Falls du auf Probleme stoßen solltest können dir die folgenden Befehle helfen die Ursache zu finden.

.. attention:: Vergewissere dich, dass die Kanalberechtigungen es **CouchBot** erlauben Posts zu verfassen!

+-------------+----------------------------------+-----------------------------------------------------------------+
| Name        | Beispiel                         | Verwendung                                                      |
+-------------+----------------------------------+-----------------------------------------------------------------+
| ping        | ``!cb ping``                     | Sollte ein "*pong*" als Antwort erhalten.                       |
+-------------+----------------------------------+-----------------------------------------------------------------+
| permissions | ``!cb permissions #ChannelName`` | Überprüft die Berechtigungen des Bots in dem angegebenen Kanal. |
+-------------+----------------------------------+-----------------------------------------------------------------+
| prefix      | ``@CouchBot#7169 prefix``        | Verräte dir den für **CouchBot** verwendeten Präfix.            |
+-------------+----------------------------------+-----------------------------------------------------------------+
| uptime      | ``!cb uptime``                   | Zeigt die Uptime des Bots.                                      |
+-------------+----------------------------------+-----------------------------------------------------------------+
