.. _youtube:

=============
YouTube Setup
=============

.. caution:: Please ensure you have read through the :ref:`Basic Config <basicconfig>` before moving to this section
             This avoids issues such as the bot not announcing anyone.

YouTube has the unique ability to indefinently store your Live Streams to VOD as well as upload your own content without the need to be Live at all.
**CouchBot**, in turn, will allow you to announce Live, VOD and/or both to your Discord servers!

.. Important:: To remove a creator, run the command again!

.. Caution:: To get your YouTube Channel ID see `this guide <https://youtube.com/account_advanced>`_.
             It's 24 characters long and starts with UC.
             Alternatvely, use the ``!cb ytidlookup`` command.

--------------
Live Streaming
--------------

Unlike other platforms, YouTube uses a Channel ID as the unique identifier for links and as such you need to know this when adding a
creator to CouchBot.

.. list-table:: Live Streaming
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel live``
     - Adds a creator to your list to announce when Live.
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel both``
     - Adds a creator to your list to announce when Live and/or Published.

----------------
Published Videos
----------------

YouTube is known for it's Video content moreso than the Live content it also offers.
To announce when a creator has uploaded a video you would use the following command;

.. list-table:: Published Videos
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel vod``
     - Adds a creator to your list to announce when a video is published.
   * - youtube
     - ``!cb youtube UC1VkELEdx28lgBg_MBkfcwQ #discord-channel both``
     - Adds a creator to your list to announce when Live and/or Published.
