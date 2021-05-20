.. _basicconfig:

===================
Grundlegende Konfiguration
===================

-------------
Admins hinzufügen
-------------

.. note:: All diese Befehle sind ein/aus Schalter. Wenn du eine Person/eine Gruppe von der Liste entfernen möchtest führe einfach den entsprechenden Befehl ein zweites Mal aus.

Nur Personen, die in der **Admin Liste** sind können Content Creators manuell zum Bot hinzufügen oder entfernen. Admins können entweder über Rollen oder als individuelle User zugewiesen werden. Beispiele für die Verwendung findest du hier:

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - admin
     - ``!cb admin @MattTheDev#0001``
     - Fügt einen individuellen User als Admin hinzu.
   * - admin
     - ``!cb admin @Developers``
     - Fügt eine Rolle als Admin hinzu.
   * - admin list
     - ``!cb admin list [page #]``
     - Zeigt eine Liste der Bot Admins an. Zeigt eine Liste der bot Admins an. Page # ist optional, der Standardwert ist 1.

----------------
Erlaubte Einstellungen
----------------

Um den Bot effektiv verwenden zu können musst du ihm mitteilen, was genau er tun soll. Beispiele dafür wären etwa veröffentlichte Videos anzukündigen oder neue Leute, die deinem Server beitreten, zu begrüßen. Einige dieser Einstellungen, wie beispielsweise der **Allow Live/Published** Befehl, sind notwendig, damit andere Teile des Bots funktionieren.

~~~~~~~~~~~~~~~~
Live & Published
~~~~~~~~~~~~~~~~

.. Caution:: Wenn nicht zumindest eine dieser Einstellungen aktiviert wird, wird der Bot garnichts ankündigen.

Die folgenden Befehle konfigurieren, ob der Bot live und / oder veröffentlichten Content ankündigen soll. Wenn du nicht zumindest eine dieser Einstellungen aktivierst wird der Bot keine Ankündigungen posten.

.. note:: Die folgenden Variablen sind sowohl in Nachrichten für **live** und **veröffentlichte** Benachrichtigungen verfügbar:
.. code-block:: none

    %TITLE% - Name des Streams
    %GAME% - Funktioniert nicht für YouTube
    %CHANNEL% - Name des Kanals
    %URL% - Vollständige URL des Streams

.. list-table:: Live
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - allow live
     - ``!cb allow live``
     - Aktiviert/Deaktiviert die Funktionen für die Ankündigungen von live Streamern.
   * - message live
     - ``!cb message live "Deine individuelle live Benachrichtigung."``
     - Legt die standard live Benachrichtigung für den Server fest.

.. list-table:: Published
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - allow published
     - ``!cb allow published``
     - Aktiviert/Deaktiviert die Funktionen für die Ankündigungen von veröffentlichten Videos.
   * - message published
     - ``!cb message published "Deine individuelle VOD Benachrichtigung."``
     - Legt die standard VOD Benachrichtigung für den Server fest.

~~~~~~~~~~~~~~~~~~~~
Begrüßungen & Verabschiedungen
~~~~~~~~~~~~~~~~~~~~

Diese Befehle erlauben es dir die Begrüßungs/Verabschiedungs Funktionen von CouchBot zu aktivieren, die ausgelöst werden, wenn neue Mitglieder deinem Server beitreten oder ihn verlassen.

.. note:: Die folgenden Variablen können hier benutzt werden:
.. code-block:: none

    %USER%
    %RANDOMUSER%

.. list-table:: Begrüßungen
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - allow greetings
     - ``!cb allow greetings``
     - Aktiviert/Deaktiviert Begrüßungen wenn eine neue Userin dem Server beitritt.
   * - channel greetings
     - ``!cb channel greetings #discord-channel``
     - Legt den Kanal für die Begrüßungs Nachrichten fest.
   * - message greeting
     - ``!cb message greeting "Deine individuelle Begrüßungs Nachricht."``
     - Legt die Begrüßungs Nachricht für den Server fest.

.. list-table:: Verabschiedungen
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - allow goodbyes
     - ``!cb allow goodbyes``
     - Aktiviert/Deaktiviert Verabschiedungen wenn ein User den Server verlässt.
   * - channel goodbyes
     - ``!cb channel goodbyes #discord-channel``
     - Legt den Kanal für die Verabschiedungs Nachrichten fest.
   * - message goodbye
     - ``!cb message goodbye "Deine individuelle Verabschiedungs Nachricht."``
     - Legt die Verabschiedungs Nachricht für den Server fest.

----------------------
Sonstige Einstellungen
----------------------

Einige weitere Einstellungen von **CouchBot** ermöglichen ein individuelleres und saubereres Setup.

Die folgenden Einstellungen verändern das Aussehen der eingebetteten Nachrichten:

.. list-table:: Zusätzliche Einstellungen der eingebetteten Nachrichten 
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - allow thumbnails
     - ``!cb allow thumbnails``
     - Fügt der eingebetteten Nachricht des Streams ein Vorschaubild hinzu.
