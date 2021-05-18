.. _customannouncements:

===============================
Individuelle Benachrichtigungen
===============================

.. caution:: Stelle bitte sicher, dass du die :ref:`Grundlegende Konfiguration <basicconfig>` gelesen hast, bevor du mit diesem Abschnitt weitermachst.
             Damit kannst du verhindern, dass der Bot beispielsweise keine Stream-Benachrichtigungen ankündigt.

Ein häufige Anfrage war es eine Möglichkeit zu schaffen, dass unterschiedliche Content Creators in unterschiedlichen Kanälen mit unterschiedlichen Rollen-Benachrichtigungs Einstellungen angekündigt werden können.
Wenn dies auch theoretisch machbar gewesen wäre wurde letztendlich entschieden eine etwas andere Lösung für CouchBot zu finden, die zum gleichen Ergebnis führt.
Anstatt zusätzliche Befehle für unterschiedliche Benachrichtigungen zu schreiben erlaubt couchBot es die Nachricht, mit der Angekündigt wird, dass jemand live geht, zu bearbeiten und in dieser Nachricht individuelle Personen und/oder Rollen zu pingen.

**Das Format für die Benachrichtigungen ist über alle Streaming Plattformen die CouchBot ankündigt das selbe.**

Wenn du einen Content Creator hinzufügst legst du gleichzeitig auch die entsprechende individuelle Benachrichtigung fest.

**z.B.:** ``!cb twitch MattTheDev #discord-channel "Der Entwickler von **CouchBot** ist gerade live!"``

Um die Benachrichtigung zu bearbeiten führe den Befehl einfach nochmal mit der neuen, überarbeiteten Benachrichtigung aus.

.. note:: Die folgenden Variablen sind sowohl in Nachrichten für **live** und **veröffenltichte** Benachrichtigungen verfügbar:
.. code-block:: none

    %TITLE% - Name des Streams
    %GAME% - Funktioniert nicht für YouTube
    %CHANNEL% - Name des Kanals
    %URL% - Vollständige URL des Streams
