.. _youtube:

=============
YouTube Setup
=============

.. caution:: Stelle bitte sicher, dass du die :ref:`Grundlegende Konfiguration <basicconfig>` gelesen hast, bevor du mit diesem Abschnitt weitermachst.
             Damit kannst du verhindern, dass der Bot beispielsweise keine Stream-Benachrichtigungen ankündigt.

Auf YouTube hochgeladene Live Streams werden unbegrenzt lange als VODs gespeichert. Auch können hier Videos hochgeladen werden, ohne überhaupt live zu gehen.
**CouchBot** erlaubt es dir, sowohl Live Content als auch VODs - oder auch beides - in deinem Discord Server anzukündigen!

.. Important:: Um einen Content Creator zu entfernen führe den Befehl ein zweites Mal aus.

.. Caution:: Um deine YouTube Kanal ID herauszufinden, folge bitte `dieser Anleitung <https://youtube.com/account_advanced>`_.
             Die ID besteht aus 24 Zeichen und beginnt mit UC.
			 Alternativ kannst du auch den Befehl ``!cb ytidlookup`` benutzen.

--------------
Live Streaming
--------------

Im Gegensatz zu anderen Plattformen benutzt YouTube eine Kanal ID als den einzigartigen Identifikator für Links, weshalb es notwendig ist
dass du diese ID kennst, wenn du einen Content Creator zu CouchBot hinzufügst.

.. list-table:: Live Streaming
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel live``
     - Fügt eine Content Creatorin zur Liste der Userinnen hinzu, deren Live Streams angekündigt werden sollen.
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel both``
     - Fügt einen Content Creator zur Liste der User hinzu, deren Live Streams und/oder veröffentlichte Videos angekündigt werden sollen.

----------------------
Veröffentlichte Videos
----------------------

YouTube ist eher für den Video-Content als für den Live-Content bekannt, der auf der Plattform angeboten wird.
Um anzukündigen, wenn eine Content Creatorin ein Video veröffentlich hat benutze bitte folgenden Befehl:

.. list-table:: Veröffentlichte Videos
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel vod``
     - Fügt einen Content Creator zur Liste der User hinzu, deren veröffentlichte Videos angekündigt werden sollen.
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel both``
     - Fügt eine Content Creatorin zur Liste der Userinnen hinzu, deren Live Streams und/oder veröffentlichte Videos angekündigt werden sollen.
