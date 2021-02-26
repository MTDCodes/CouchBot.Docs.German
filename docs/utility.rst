.. _utility:

=========
Utilities
=========

---------------
Custom Commands
---------------

Custom commands allow a versatile way for you to have the bot respond to different terms.
This could be used to advertise your Twitter, display your Discord invite or have the bot ping someone!

.. list-table:: Custom Commands
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - command add
     - ``!cb command add "CouchMe" 5 "You have been Couched!"``
     - Creates a command called ``CouchMe`` with a 5 second cooldown that replies *"You have been Couched!"*
   * - command remove
     - ``!cb command remove "CouchMe"`` 
     - Removes the command, in this instance ``CouchMe``.
   * - command list
     - ``!cb command list``
     - Displays a list of the current commands you have programmed.

----------
Moderation
----------

This provides basic moderation actions that can be used via the bot;

.. list-table:: Moderation Commands
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - kick
     - ``!cb kick @MattTheDev#0001``
     - Kicks the user from the server.
   * - ban
     - ``!cb ban @MattTheDev#0001``
     - Bans the user from the server.
   * - echo
     - ``!cb echo Matt is Great!``
     - Gets the CouchBot to repeat the text you specify.

--------------------
Random Announcements
--------------------

Ever wanted to put a random stream in a channel? Of course you did and now you can!

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - announce random 
     - ``!cb announce random twitch``
     - Will announce a random stream in the channel you type it in (**Admin Only**)
   * - dm random
     - ``!cb dm random twitch``
     - Will DM a random stream to the user that ran the command.

-------------
Misc Commands
-------------

Use the following commands to configure and view various other bits and bobs.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - info 
     - ``!cb info``
     - Brief stats overview of the bot.
   * - invite
     - ``!cb invite``
     - Sends you a message with the bot invite.
   * - ytidlookup 
     - ``!cb ytidlookup "Channel Name"``
     - Tries to locate the channel ID for YouTube.
   * - whatsthis
     - ``!cb whatsthis``
     - Give a link to an image to find out.
   * - config list 
     - ``!cb config list``
     - Gives a link to the bots configuration.
   * - config deleteoffline
     - ``!cb config deleteoffline``
     - Deletes offline streams.
   * - config textannouncements
     - ``!cb config textannouncements``
     - Announces in text rather than embeds
   * - clap 
     - ``!cb clap place your text here``
     - Places a clap in all the spaces.
   * - cookie
     - ``!cb cookie place your text here``
     - Places a cookie in all the spaces.
   * - clone
     - ``!cb clone #ChannelClone All notifications go in here.``
     - You can use this command to clone a channel and pin the message you specify.
   * - prefix
     - ``!cb prefix -``
     - Using the command like this will change your prefix to ``-``

-----------------------
Purge (Delete) Messages
-----------------------

Sometimes you may wish to clear channels, messages or just messages from specific people to help in the effective
moderation of you server. To accomplish this you can use the following commands.

.. Warning:: You must have **Manage Messages** permissions to run this command!
			 Once run, you will be unable to restore deleted messages.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - purge 
     - ``!cb purge``
     - Deletes 100 messages in the current channel.
   * - purge
     - ``!cb purge 25``
     - This would purge 25 messages in the current channel.
   * - purge 
     - ``!cb purge 25 #DiscordChannel``
     - This would purge 25 messages in the channel #DiscordChannel.
   * - purge
     - ``!cb purge 25 #DiscordChannel true``
     - This would purge 25 messages in the channel #DiscordChannel including pinned messages.
   * - purge
     - ``!cb purge @MattTheDev``
     - Deletes all messages from user within the last 100 messages in the current channel.
   * - purge
     - ``!cb purge @MattTheDev true``
     - Deletes all messages from user within the last 100 messages in the current channel, including pinned messages.
   * - purge
     - ``!cb purge @MattTheDev #DiscordChannel``
     - Deletes all messages from user within the last 100 messages in the current channel.
   * - purge
     - ``!cb purge @MattTheDev #DiscordChannel true``
     - Deletes all messages from user within the last 100 messages in the current channel, including pinned messages.

.. Warning:: The following commands have no confirmation and will execute when run.

.. list-table:: Creator Purge
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - creators purge 
     - ``!cb creators purge``
     - Removes all manually added creators from announcing.
   * - creators purge 
     - ``!cb creators purge twitch``
     - Removes all manually added creators on Twitch from announcing, works for all platforms.
