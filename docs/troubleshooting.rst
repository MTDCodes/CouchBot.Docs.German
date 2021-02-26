.. _troubleshooting:

===============
Troubleshooting
===============

You can join the CouchBot support server at this link --> https://discord.couch.bot/

------------------------
Bot Required Permissions
------------------------

When **CouchBot** joins your server he should request all the necessary permissions when prompted to join.
To ensure that **CouchBot** can function fully on your server, please ensure all of the following permissions are granted to his server role:

- Manage Roles (For Live Discovery / Role Assignment)
- Read Text Channels (For ALL Functionality)
- Send Messages (For ALL Functionality)
- Manage Messages (For DeleteOffline Functionality)
- Embed Links (For ALL Functionality)
- Read Message History (For ALL Functionality)
- Mention Everyone (For Ping Functionality)

If you are having issues you can use the following commands to help in identifying where they are.

.. attention:: Ensure the channel also has the correct permissions to allow **CouchBot** to post!

+-------------+----------------------------------+---------------------------------------------+
| Name        | Example                          | Usage                                       |
+-------------+----------------------------------+---------------------------------------------+
| ping        | ``!cb ping``                     | Should provide a "*pong*" response.         |
+-------------+----------------------------------+---------------------------------------------+
| permissions | ``!cb permissions #ChannelName`` | Checks the bots permissions in the channel. |
+-------------+----------------------------------+---------------------------------------------+
| prefix      | ``@CouchBot#7169 prefix``        | Tells you your prefix.                      |
+-------------+----------------------------------+---------------------------------------------+
| uptime      | ``!cb uptime``                   | Shows the bots uptime.                      |
+-------------+----------------------------------+---------------------------------------------+
