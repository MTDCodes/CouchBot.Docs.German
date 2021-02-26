.. _customannouncements:

====================
Custom Announcements
====================

.. caution:: Please ensure you have read through the :ref:`Basic Config <basicconfig>` before moving to this section
             This avoids issues such as the bot not announcing anyone.

A common request was to allow different creators to be announced in different channels with different role ping settings.
Whilst we could theoretically do this it was decided to partly bring this into play within CouchBot.
Rather than hardcode in additional commands for pinging people, we allow you to edit the message when someone goes live allowing you to ping
whatever role/person you choose.

**The format for this is the same across all streaming platform that CouchBot announces.**

When adding a creator you would specify the custom message at the same time;

**e.g.** ``!cb twitch MattTheDev #discord-channel "The Developer of **CouchBot** has gone live!"``

Editing the message is as simple as running the command again with the new message to be announced.

.. note:: The following variables are available to use in the **Live** and **Published** messages.
.. code-block:: none

    %TITLE% - Name of the Stream
    %GAME% - Not working for YouTube
    %CHANNEL% - Channel Name
    %URL% - Full URL of the Stream
