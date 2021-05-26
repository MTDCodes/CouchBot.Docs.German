.. _rolemanagement:

===============
Rollenzuweisung
===============

**CouchBot** ist in der Lage Rollen basierend auf verschiedenen Kriterien zuzuweisen. Beispiele dafür wären etwa, dass eine Userin dem Server beitritt oder einen Befehl in Discord eingibt.
So können beispielsweise Benachrichtigungen wenn Content Creators live gehen erhalten werden, indem man "*Ich liebe Streams*" als Befehl verwendet.

.. caution:: Wenn du Rollen zuweisen möchtest stelle sicher, dass der Bot eine höhere Rolle in Discord hat als die Rolle, die er vergeben soll.

Wenn du möchtest, dass Usern eine Rolle zugewiesen wird wenn sie deinem Discord Server beitreten dann benutze die folgenden Befehle:

.. list-table:: Server Beitritts Befehle
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - role join 
     - ``!cb role join @RoleName``
     - Weist eine Rolle zu wenn Userinnen deinem Server beitreten.
   * - role join reset 
     - ``!cb role join reset``
     - Resetted die Server Beitrittsrolle zurück zu nichts.

Damit Userinnen einen bestimmten Ausdruck im Chat verwenden können, um sich selbst Rollen zuzuweisen, gehe wie folgt vor:

.. list-table:: Chat Ausdruck Befehle
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - role add 
     - ``!cb role add "CouchMe" [add/remove] @RoleTheyGet``
     - Fügt eine Rolle hinzu (add)/Entfernt eine Rolle (remove) wenn jemand "**CouchMe**" eintippt
   * - role remove 
     - ``!cb role remove "CouchMe"`` 
     - Entfernt den "CouchMe" Befehl.

Es können auch Rollen basierend auf Reaktionen hinzugefügt werden, wenn du das bevorzugst oder einfacher zu implementieren findest:

.. Note:: Eine *einzelne* Reaktions-Nachricht kann bis zu **vier** Reaktions-Rollen beinhalten. Solltest du mehr als 4 Rollen benötigen verfasse bitte weitere Reaktions-Nachrichten.

.. list-table:: Reaktions Rollen Befehle
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Beispiel
     - Verwendung
   * - rm 
     - ``!cb rm @Streamer :thumbsup: Please react to get the Streamer role!``
     - Fügt eine Rolle hinzu oder entfernt sie wenn jemand mit dem :thumbsup: Emoji reagiert."
   * - rm 
     - ``!cb rm @Streamer :thumbsup: @Announcements :loudspeaker: Please react to get the desired role!``
     - Fügt eine Rolle hinzu oder entfernt sie wenn jemand mit dem :thumbsup: und/oder :loudspeaker: Emoji reagiert."

Dle letzte verfügbare Rollen Option funktioniert nur in Verbindung mit Twitch und fügt einer Person die gerade live ist eine spezielle Rolle **für den Zeitraum des Livestreams** hinzu.
Nähere Informationen zu dieser Rolle findest du in der :ref:`Twitch Info <twitch>`.
