.. _messages:

==============
Advanced Messages Setup
==============

.. caution:: If you are looking to setup messages per creator then follow the instructions in the :ref:`Custom Announcements <customannouncements>` section.

Use the following commands to configure custom message options and test them.

.. note:: The following variables are available to use in the **Live** and **Published** messages.
.. code-block:: none

    %TITLE% - Name of the Stream
    %GAME% - Not working for YouTube
    %CHANNEL% - Channel Name
    %URL% - Full URL of the Stream

.. note:: The following variables are available to use in the **Greetings** and **Goodbye** messages.
.. code-block:: none

    %USER%
    %RANDOMUSER%

+-------------------+---------------------------------------------------------+-----------------------------------------------+
| Name              | Example                                                 | Usage                                         |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message live      | ``!cb message live "Your Custom Live Message"``         | Changes your live message for the server.     |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message published | ``!cb message published "Your Custom VOD Message"``     | Changes your VOD message for the server.      |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message offline   | ``!cb message offline "Your Custom Offline Message"``   | Changes your offline message for the server.  |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message greeting  | ``!cb message greeting "Your Custom Greeting Message"`` | Changes your greeting message for the server. |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message goodbye   | ``!cb message goodbye "Your Custom Goodbye Message"``   | Changes your goodbye message for the server.  |
+-------------------+---------------------------------------------------------+-----------------------------------------------+

If you want to reset your greetings and messages (or not change them) to the default ones, use the following commands;

+--------------------+----------------------------------+--------------------------------------------------------+
| Name               | Example                          | Usage                                                  |
+--------------------+----------------------------------+--------------------------------------------------------+
| message live       | ``!cb message live clear``       | Resets your live message for the server.               |
+--------------------+----------------------------------+--------------------------------------------------------+
| message published  | ``!cb message published clear``  | Resets your VOD message for the server.                |
+--------------------+----------------------------------+--------------------------------------------------------+
| message offline    | ``!cb message offline clear``    | Resets your offline message for the server.            |
+--------------------+----------------------------------+--------------------------------------------------------+
| message greeting   | ``!cb message greeting clear``   | Resets your greeting message for the server.           |
+--------------------+----------------------------------+--------------------------------------------------------+
| message goodbye    | ``!cb message goodbye clear``    | Resets your goodbye message for the server.            |
+--------------------+----------------------------------+--------------------------------------------------------+
| message offline    | ``!cb message offline ""``       | Leaves the original announcement post without changes. |
+--------------------+----------------------------------+--------------------------------------------------------+

To have the message outside of the embed blank, use the following;

+-------------------+---------------------------------+--------------------------------------------------------------+
| Name              | Example                         | Usage                                                        |
+-------------------+---------------------------------+--------------------------------------------------------------+
| message live      | ``!cb message live empty``      | Remove message outside of embed on live stream announcement. |
+-------------------+---------------------------------+--------------------------------------------------------------+
| message published | ``!cb message published empty`` | Remove message outside of embed on published announcement.   |
+-------------------+---------------------------------+--------------------------------------------------------------+

If you want to test your messages, use the following commands;

+-------------------+----------------------------------------+----------------------------------------------+
| Name              | Example                                | Usage                                        |
+-------------------+----------------------------------------+----------------------------------------------+
| test live         | ``!cb test live #DiscordChannel``      | Tests your live message for the server.      |
+-------------------+----------------------------------------+----------------------------------------------+
| test published    | ``!cb test published #DiscordChannel`` | Tests your VOD message for the server.       |
+-------------------+----------------------------------------+----------------------------------------------+
| test greeting     | ``!cb test greeting``                  | Tests your greeting message for the server.  |
+-------------------+----------------------------------------+----------------------------------------------+
| test goodbye      | ``!cb test goodbye``                   | Tests your goodbye message for the server.   |
+-------------------+----------------------------------------+----------------------------------------------+
