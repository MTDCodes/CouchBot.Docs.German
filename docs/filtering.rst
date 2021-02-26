.. _filtering:

=========
Filtering
=========

.. note:: These commands are toggled, if you want to remove something from the list, run the command again.

**CouchBot** has the ability to filter announcements to specific games, stream titles.
This will only allow items mentioned on this list to be announced regardless of what creators you may have added.
An example being if someone played Destiny 2 they would never be announced in the following examples.

.. list-table:: Filter Commands
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - filter game
     - ``!cb filter game twitch "World of*"``
     - Creates a **Game Filter** on Twitch for any games starting with "World of"
   * - filter title
     - ``!cb filter title twitch "World of*"``
     - Creates a **Stream Title Filter** on Twitch for any titles starting with "World of"
   * - filter list
     - ``!cb filter list``
     - Displays a list of the current applicable filters.
