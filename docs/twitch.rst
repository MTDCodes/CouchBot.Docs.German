.. _twitch:

============
Twitch Setup
============

.. caution:: Please ensure you have read through the :ref:`Basic Config <basicconfig>` before moving to this section
             This avoids issues such as the bot not announcing anyone.

Twitch is by far the most popular streaming platform in the world at the time of this writing.
Being the market leader, it has some integrations which make announcing in Discord much easier to setup en mass.

---------------
Live Discovery
---------------

.. DANGER:: This requires that there is **No Custom Status** set and the person streaming has the "**Purple Dot**"

**CouchBot** has the ability to **automatically discover** people in your Discord server that are streaming to **Twitch**.
This is done via the purple "*Streaming*" indicator on a persons profile when they stream using OBS or similar triggering *Streamer Mode* on Discord.

The following table shows the only steps needed to configure this for immediate use in your server;

.. list-table:: Basic Live Discovery Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - channel live
     - ``!cb channel live #discord-channel``
     - This channel will be where Discovery announcements go.
   * - allow livediscovery
     - ``!cb allow livediscovery all``
     - Allows the automatic announcing of people with the status of “Streaming”.

You can also limit the people that will be announced using assigned roles or you can switch this feature off completely;

.. list-table:: Advanced Live Discovery Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow livediscovery
     - ``!cb allow livediscovery none``
     - Prevents the automatic announcing of people with the status of “Streaming”.
   * - allow livediscovery
     - ``!cb allow livediscovery role @Streamer`` 
     - Allows the automatic announcing of people with the status of “Streaming” and the role of @Streamer.

Finally, Live Discovery also allows you to assign a "**Live Now**" type role to creators allowing you to hoist them to show current
live users in your server. The role will only be added when they are **Live** then **Removed** when they are finished automatically.
The command for this feature is as follows;

.. list-table:: Live Discovery Roles Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - role live
     - ``!cb role live @RoleTheyGet``
     - The role that gets **assigned** to a person when they go live.

-----------------------
Manually Add Creator(s)
-----------------------

Manually adding creators allows a fine grained level of control over who is announed in your server and allows things such as custom announcements and channels
to be selected giving much more options on who should be announced and where.
This is particularly useful on a creators server where they may want to use **@here** to announce when they are live but not for anyone else.

For more information on custom messages please see :ref:`Custom Announcements <customannouncements>`

.. Important:: To remove a creator, run the command again!

.. list-table:: Manual Twitch Setup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - twitch
     - ``!cb twitch MattTheDev #discord-channel``
     - Adds a creator be announced
