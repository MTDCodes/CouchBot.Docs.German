.. _twitch:

============
Twitch Setup
============

.. caution:: Stelle bitte sicher, dass du die :ref:`Grundlegende Konfiguration <basicconfig>` gelesen hast, bevor du mit diesem Abschnitt weitermachst.
             Damit kannst du verhindern, dass der Bot beispielsweise keine Stream-Benachrichtigungen ankündigt.

Zum Zeitpunkt des Erstellens dieser Dokumentaton its Twitch die bei weitem populärste Streaming Plattform.
Als Marktführer hat Twitch daher einige Integrationen, die das Einrichten von Benachrichtigungen in Discord en masse einfacher machen.

---------------
Live Discovery
---------------

.. DANGER:: Hierfür ist es notwendig, dass in Discord **kein personalisierter Status** gesetzt ist und bei der Streamerin in Discord der **lila Punkt** zu sehen ist.

**CouchBot** kann Personen, die in deinem Discord Server sind und auf **Twitch** streamen **automatisch zu erkennen.**
Das wird anhand des lila "*Streaming*" Indikators ermöglicht, der beim Profil einer Person aufscheint, wenn diese mittels OBS oder anderer Software streamed und den *Streamer Modus* aktiviert hat.

Die folgende Tabelle zeigt die Befehle die notwendig sind, um diese Funktion sofort in deinem Server nutzen zu können:

.. list-table:: Grundlegendes Live Discovery Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - channel live
     - ``!cb channel live #discord-channel``
     - Dies liegt den Kanal fest, in welchen Live Discovery Benachrichtigungen geschickt werden.
   * - allow livediscovery
     - ``!cb allow livediscovery all``
     - Erlaubt dass automatisch Benachrichtigungen geschickt werden, wenn eine Person den Discord Sreamer Modus aktiviert.

Du kannst mittels Rollen auch einschränken, für welche Personen Benachrichtigungen erstellt werden oder dieses Feature vollständig deaktivieren.

.. list-table:: Fortgeschrittenes Live Discovery Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow livediscovery
     - ``!cb allow livediscovery none``
     - Verhindert dass automatische Benachrichtigungen geschickt werden, wenn eine Person den Discord Streamer Modus aktiviert.
	    * - allow livediscovery
     - ``!cb allow livediscovery role @Streamer`` 
     - Erlaubt dass automatisch Benachrichtigungen geschickt werden, wenn eine Person den Discord Sreamer Modus aktiviert und die Rolle @Streamer hat.
	 

Zu guter Letzt ermöglicht es dir Live Discovery, Content Creators eine "**Jetzt Live**" Rolle zuzuweisen, die sie in der Benutzerliste 
deines Servers hervorhebt. Diese Rolle wird nur hinzugefügt, wenn ein Streamer **live** ist und automatisch wieder **entfernt** wenn der Stream beendet wurde.
Der Befehl dafür lautet wie folgt:

.. list-table:: Live Discovery Rollen Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - role live
     - ``!cb role live @RoleTheyGet``
     - Diese Rolle wird für die Zeit des Livestreams **hinzugefügt.**

-----------------------------------
Content Creators manuell hinzufügen
-----------------------------------

Das manuelle Hinzufügen von Content Creators erlaubt detailierte Kontrolle darüber, wessen Streams in deinem Server angekündigt werden, in welchen Kanälen 
und mit welchen Nachrichten. 
Das ist besonders in den Servern von Content Creators nützlich, die nur ihre eigenen Streams mit **@here** ankündigen wollen, andere Streams jedoch etwas subtiler.

Nähere Informationen zu individualisierten Benachrichtigungen findest du unter :ref:`Individuelle Benachrichtigungen <customannouncements>`

.. Important:: Um einen Content Creator zu entfernen führe den Befehl ein zweites Mal aus.

.. list-table:: Manual Twitch Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - twitch
     - ``!cb twitch MattTheDev #discord-channel``
     - Fügt einen Content Creator zur Liste der anzukündigenden Streamer hinzu.
