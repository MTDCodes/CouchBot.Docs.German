.. _messages:

===================================
Fortgeschrittenes Nachrichten Setup
===================================

.. caution:: Wenn du Benachrichtigungen für einzelne Content Creators hinzufügen möchtest, folge den Anweisungen im :ref:`Individuelle Benachrichtigungen <customannouncements>` Bereich.

Mit den folgenden Befehlen kannst du individuelle Benachrichtigungen konfigurieren und testen.

.. note:: Die folgenden Variablen sind sowohl in Nachrichten für **live** und **veröffenltichte** Benachrichtigungen verfügbar:
.. code-block:: none

    %TITLE% - Name des Streams
    %GAME% - Funktioniert nicht für YouTube
    %CHANNEL% - Name des Kanals
    %URL% - Vollständige URL des Streams

.. note:: Die folgenden Variablen sind in **Begrüßungs** Nachrichten verfügbar:
.. code-block:: none

    %NEWLINE% - Neue Zeile einfügen.
	%NICKNAME% - Spitzname der Person, die dem Server beigetreten ist. Falls kein Spitzname vergeben ist wird der Benutzername verwendet.
	%RANDOMUSER% - Zufälliger Benutzername des Servers.
	%SERVER% - Name des Servers.
	%SERVERID% - ID des Servers.
	%TIMESTAMPUTC% - Aktuelle Uhrzeit in UTC
	%USER% - Benutzername der Person, die dem Server beigetreten ist.
	%USERID% - Benutzer ID der Person, die dem Server beigetreten ist.
	
.. note:: Die folgenden Variablen sind in **Verabschiedungs** Nachrichten verfügbar:
.. code-block:: none

	%HOWLONG% - Menschlich lesbare Verweildauer am Server, z.B.: 3 monate, 2 tage und 6 Stunden.
	%JOINDATE% - Das Datum, an dem die verlassende Person dem Server ursprünglich beigetreten ist.
	%NEWLINE% - Neue Zeile einfügen.
	%NICKNAME% - Spitzname der Person, die den Server verlässt. Falls kein Spitzname vergeben ist wird der Benutzername verwendet.
	%RANDOMUSER% - Zufälliger Benutzername des Servers.
	%SERVER% - Name des Servers.
	%SERVERID% - ID des Servers.
	%TIMESTAMPUTC% - Aktuelle Uhrzeit in UTC
	%USER% - Benutzername der Person, die den Server verlässt.
	%USERID% - Benutzer ID der Person, die den Server verlässt.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - message live
     - ``!cb message live "Deine individuelle live Benachrichtigung."``
     - Legt die standard live Benachrichtigung für den Server fest.
   * - message published
     - ``!cb message published "Deine individuelle VOD Benachrichtigung."``
     - Legt die standard VOD Benachrichtigung für den Server fest.
   * - message offline
     - ``!cb message offline "Deine individuelle offline Benachrichtigung."``
     - Legt die offline Benachrichtigung für den Server fest.
   * - message greeting
      - ``!cb message greeting "Deine individuelle Begrüßungs Nachricht."``
      - Legt die Begrüßungs Nachricht für den Server fest.
   * - message goodbye
      - ``!cb message goodbye "Deine individuelle Verabschiedungs Nachricht."``
      - 	Legt die Verabschiedungs Nachricht für den Server fest.

Wenn du Begrüßungen oder andere Nachrichten auf die Standardwerte zurücksetzen möchtest benutze folgende Befehle:

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - message live
     - ``!cb message live clear``
     - Setzt die live Benachrichtigung des Servers auf den Standardwert zurück.
   * - message published
     - ``!cb message published clear``
     - Setzt die VOD Benachrichtigung des Servers auf den Standardwert zurück.
   * - message offline
     - ``!cb message offline clear``
     - Setzt die offline Benachrichtigung des Servers auf den Standardwert zurück.
   * - message greeting
      - ``!cb message greeting clear``
      - Setzt die Begrüßungs Nachricht des Servers auf den Standardwert zurück.
   * - message goodbye
      - ``!cb message goodbye clear``
      - Setzt die Verabschiedungs Nachricht des Servers auf den Standardwert zurück.
   * - message offline
      - ``!cb message offline ""``
      - Lässt die ursprüngliche Benachrichtigung ohne Veränderung bestehen.

Um die Nachrichten, die vor den eingebetten Nachrichten stehen, leer zu lassen, verwende folgende Befehle:

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - message live
     - ``!cb message live empty``
     - Entfernt Nachrichten außerhalb der eingebetteten live Benachrichtigungen.
   * - message published
     - ``!cb message published empty``
     - Entfernt Nachrichten außerhalb der eingebetteten VOD Benachrichtigungen.

Wenn du deine Benachrichtigungen testen möchtest verwende folgende Befehle:

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - test live
     - ``!cb test live #DiscordChannel``
     - Testet die live Benachrichtigung für deinen Server.
   * - test published
     - ``!cb test published #DiscordChannel``
     - Testet die VOD Benachrichtigung für deinen Server.
   * - test greeting
     - ``!cb test greeting``
     - Testet die Begrüßungs Nachricht für deinen Server.
   * - test goodbye
      - ``!cb test goodbye``
      - Testet die Verabschiedungs Nachricht für deinen Server.
	 
