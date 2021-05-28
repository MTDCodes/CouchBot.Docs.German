.. _examples:

===============
Setup Beispiele
===============

In diesen Szenarios haben wir die :ref:`Grundlegende Konfiguration <basicconfig>` bereits durchgeführt und dem Bot die benötigten :ref:`Berechtigungen <troubleshooting>` gegeben.
Wir werden ``MatttheDev`` als Streamer Account und ``#notification`` als den zu verwendenden Discord Kanal verwenden.

-----------
Szenario 1
-----------

.. admonition:: Szenario 1

   Das **live** Gehen des Serverbesitzers mit einer Benachrichtigung an alle User des Servers ankündigen.


Viele Leute wollen einfach nur, dass der Bot ankündigt, wenn sie live gehen. CouchBot kann das natürlich!
Wir geben dem Bot zunächst die Berechtigungen live Streams anzukündigen und fügen anschließend den Content Creator hinzu.
Dann sagen wir dem Bot dass er die everyone Rolle pingen soll.

.. code-block:: none

    !cb allow live
    !cb twitch MattTheDev #notification "Der Dev ist jetzt live @everyone"

-----------
Szenario 2
-----------

.. admonition:: Szenario 2

   Streams automatisch ankündigen ohne Content Creatorinnen individuell hinzuzufügen.

Anstatt Personen einzeln manuell hinzuzufügen kann der Bot auch automatisch erkennen wenn User deines Servers live gehen.
Das reduziert die Zeit für das Einrichten drastisch und macht den Setup Prozess für dich weit einfacher.
Zunächst erlaubst du dem Bot live Benachrichtigungen zu posten und legst anschließend den Standard-Kanal für diese Benachrichtigungen fest.
Dann lässt du den Bot nach Userinnen mit dem Streaming Status Ausschau halten und bist auch schon fertig!

.. caution:: Der Streamer muss den Discord Status "Streaming" haben um automatisch angekündigt zu werden.

.. code-block:: none

    !cb allow live
    !cb channel live #notification
    !cb allow livediscovery all

-----------
Szenario 3
-----------

.. admonition:: Szenario 3

   Live Streams einer bestimmten Benutzerrolle automatisch ankündigen.

Gehen wir davon aus dass du nur live Streams von Userinnen mit der VIP Rolle ankündigen lassen möchtest. Um dies zu bewerkstelligen
erlaubst du dem Bot zunächst, live Benachrichtigungen zu posten und definierst den Kanal in dem er posten soll.
Anschließend musst du ihm nur noch sagen welche Rolle angekündigt werden soll!

.. caution:: Die Streamerin muss den Discord Status "Streaming" haben um automatisch angekündigt zu werden.

.. code-block:: none

    !cb allow live
    !cb channel live #notification
    !cb allow livediscovery role @VIP

-----------
Szenario 4
-----------

.. admonition:: Szenario 4

   Der Serverbesitzer soll separat von anderen Streamern angekündigt werden.

Manche Server möchten eventuell den Besitzer oder andere "VIPs" separat von anderen Usern ankündigen lassen.
Dafür erlauben wir CouchBot zunächst live Benachrichtigungen zu posten und fügen dann die Streamer einzeln mit dem jeweils spezifischen Kanal hinzu, in dem die Ankündigungen gepostet werden sollen.

.. code-block:: none

    !cb allow live
    !cb twitch MattTheDev #ownerchannel
    !cb twitch Jaymei #otherchannel

-----------
Szenario 5
-----------

.. admonition:: Szenario 5

   Benachrichtigungen für YouTube VODs und Live Streams in unterschiedlichen Kanälen

Zunächst erlauben wir dem Bot sowohl Benachrichtigungen für live als auch für veröffentlichten Content zu posten. Da die Befehle dafür ein/aus Schalter sind wird als Antwort die neue, jetzt gültige Einstellung geliefert.
Anschließend fügen wir den YouTube Kanal mittels der dazugehörigen "ChannelID_" sowie den jeweiligen Kanal, in dem die Benachrichtigungen für live und veröffentlichten Content gepostet werden sollen hinzu.
Es ist auch möglich diesen Teil leer zu lassen oder das Argument "both" zu verwenden, damit beide Benachrichtigungen in den selben Kanal gepostet werden.

.. _ChannelID: https://youtube.com/account_advanced

.. code-block:: none

    !cb allow live
    !cb allow published
    !cb youtube UC123456 #livechannel live
    !cb youtube UC123456 #publishedchannel vod

-----------
Szenario 6
-----------

.. admonition:: Szenario 6

   Der Serverbesitzer soll separat von anderen Streamern angekündigt werden und unterschiedliche Gruppen werden mit individuellen Nachrichten benachrichtigt.

Du möchtest @everyone benachrichtigen wenn du live gehst. Du möchtest @Streamer benachrichtigen, wenn andere Personen live gehen.
Der dritte Befehl würde die Standard Benachrichtigung für live Streams verwenden.

.. code-block:: none

    !cb twitch MattTheDev #BigNotification "@everyone CouchBot Programmierer **MattTheDev** ist jetzt online!"
    !cb twitch Jaymei #notification "@Streamer Eine weitere individuelle Nachricht!"
    !cb twitch EmElle #notification

-----------
Nachrichten
-----------

Vielleicht möchtest du ja eine individuelle Nachricht erstellen um die Leute mit **CouchBot** wissen zu lassen,
dass du live bist oder um neue Servermitglieder zu begrüßen. Die folgenden Befehle zeigen dir wie!

.. admonition:: Szenario 1

   Begrüßungs- und Verabschiedungs-Nachrichten einstellen

.. note:: Du kannst die Argumente **%USER%** und **%RANDOMUSER%** verwenden.

.. code-block:: none

    !cb allow greetings
    !cb allow goodbyes
    !cb channel greetings #channel-name
    !cb channel goodbyes #channel-name
    !cb message greeting "Deine individuelle Begrüßungs-Nachricht."
    !cb message goodbye "Deine individuelle Verabschiedungs-Nachricht"

.. admonition:: Szenario 2

   Benuzerdefinierte live Benachrichtigungen.

Du möchtest den Benachrichtigungen in deinem Server einen persönlichen Touch hinzufügen?
Hier wird dir geholfen:

.. note:: Du kannst die Argumente **%TITLE%, %GAME%, %CHANNEL% und %URL%** verwenden.

.. code-block:: none

    !cb message live "Deine benutzerdefinierte live Benachrichtigung."	
    !cb message published "Deine benutzerdefinierte VOD Benachrichtigung."
