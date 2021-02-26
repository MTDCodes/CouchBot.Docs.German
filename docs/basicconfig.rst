.. _basicconfig:

===================
Basic Configuration
===================

-------------
Assign Admins
-------------

.. note:: These commands are toggled, if you want to remove a person/group from the list, run the command again.

In order for people to manually add and remove content creators to the bot, they must be on the **Approved Admin List**.
They can either be added by role or by individual user, see examples below on how to configure this;

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - admin
     - ``!cb admin @MattTheDev#0001``
     - Adds an individual to admin.
   * - admin
     - ``!cb admin @Developers``
     - Adds a role to administrate the bot.
   * - admin list
     - ``!cb admin list``
     - Provides a list of the configured bot admins

----------------
Allowed Settings
----------------

In order to run the bot effectively, you must tell it what you wish it to do.
An example of this can be to announce published videos only or to greet people joining your server.
Some of these settings are necessary for other areas to function such as the **Allow Live/Published** command.

~~~~~~~~~~~~~~~~
Live & Published
~~~~~~~~~~~~~~~~

.. Caution:: If you fail to set either of these the bot will announce no-one.

Use the following commands to configure whether the bot should announce live and/or published content.
If you choose not to enable either of these then the bot will in effect, not announce anything.

.. note:: The following variables are available to use in the **Live** and **Published** messages.
.. code-block:: none

    %TITLE% - Name of the Stream
    %GAME% - Not working for YouTube
    %CHANNEL% - Channel Name
    %URL% - Full URL of the Stream

.. list-table:: Live
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow live
     - ``!cb allow live``
     - Toggles allowing stream announces for live streamers.
   * - message live
     - ``!cb message live "Your Custom Live Message"``
     - Changes your live message for the server.

.. list-table:: Published
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow published
     - ``!cb allow published``
     - Toggles allowing published videos to be announced.
   * - message published
     - ``!cb message published "Your Custom VOD Message"``
     - Changes your VOD message for the server.

~~~~~~~~~~~~~~~~~~~~
Greetings & Goodbyes
~~~~~~~~~~~~~~~~~~~~

These commands allow you to enable the greeting/goodbye function of CouchBot, this will trigger when people join/leave your server.

.. note:: The following variables are available to use in this location.
.. code-block:: none

    %USER%
    %RANDOMUSER%

.. list-table:: Greetings
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow greetings
     - ``!cb allow greetings``
     - Toggle allowing greetings when a member joins the server.
   * - channel greetings
     - ``!cb channel greetings #discord-channel``
     - Sets the greeting channel.
   * - message greeting
     - ``!cb message greeting "Your Custom Greeting Message"``
     - Changes your greeting message for the server.

.. list-table:: Goodbyes
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow goodbyes
     - ``!cb allow goodbyes``
     - Toggle allowing goodbyes when a member leaves the server.
   * - channel goodbyes
     - ``!cb channel goodbyes #discord-channel``
     - Sets the goodbye channel.
   * - message goodbye
     - ``!cb message goodbye "Your Custom Goodbye Message"``
     - Changes your goodbye message for the server.

----------------------
Miscellaneous Settings
----------------------

There are a few other settings available within **CouchBot** to allow a more customised and cleaner setup.

The following settings change the apperance of the embed message;

.. list-table:: Additional Embed Settings
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - allow thumbnails
     - ``!cb allow thumbnails``
     - Adds an image to the bottom of the embed from the stream.
