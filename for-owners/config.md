# Current Configuration File

Below you can see the contents of the newest BungeeCord PlayerServers configuration file.

{% hint style="info" %}
Please note that in some extremely rare cases I may **forget to update the config** on this page.
{% endhint %}

```yaml
#  __________.__                             _________
#  \______   \  | _____  ___.__. ___________/   _____/ ______________  __ ___________  ______
#  |     ___/  | \__  \<   |  |/ __ \_  __ \_____  \_/ __ \_  __ \  \/ // __ \_  __ \/  ___/
#  |    |   |  |__/ __ \\___  \  ___/|  | \/        \  ___/|  | \/\   /\  ___/|  | \/\___ \
#  |____|   |____(____  / ____|\___  >__| /_______  /\___  >__|    \_/  \___  >__|  /____  >
#                     \/\/         \/             \/     \/                 \/           \/
#
# An advanced plugin which allows your players to create their own sub-servers, created by thearcadia.xyz

# Please enter your MySQL information below.
mysql:
  hostname: 127.0.0.1
  username: web
  password: webmaster
  database: playerservers

# This setting defines port range
ports:
  start-port: 30000
  end-port: 40000

build-tools:
  # Should we log build-tools console output? Highly recommended to set
  # to true, as it will help me a lot with potential issues.
  build-tools-debug: true

  # What version should we build for PlayerServers?
  # Do "latest" for latest, do "1.8.8" for 1.8.8, etc.
  # If you want to change the sub-servers version,
  # you will have to delete templates/Spigot.jar first,
  # and than reboot the server. Btw, it is highly
  # recommended to use 1.8.8 for sub-servers.
  #
  # ALSO, KEEP IN MIND THAT 1.8.8 SERVERS WILL NOT
  # BUILD IF YOU HAVE JAVA 11+, ESPECIALLY JAVA 13!
  # USE JAVA 8 FOR THE BEST POSSIBLE EXPERIENCE
  build-version: "1.8.8"

# Use player-name instead of server UUID? Basically, when turned on, server-names
# will be called Mike instead of (for example) aa386b6h
# CURRENTLY EXPERIMENTAL. SWITCHING THIS OPTION AFTER HAVING PLAYERSERVERS
# COULD (but most likely won't) POTENTIALLY BREAK THE CURRENT SETUP. USE AT CAUTION.
use-usernames: false

# What is the max amount of servers that can be running at once?
max-running-instances: 15

# If there are no online players, and the last join was before
# more than minutes-to-shutdown, the server will automatically shutdown
# to allow more space for active ones.
minutes-to-shutdown: 15

# After how many seconds after executing cp -r <templatefile> <yourserverfolder>
# should we launch the server? Increase this if you get could not connect message.
copy-delay: 3

# In how much seconds, after first boot-up of the server should we
# teleport the player to their sub-server? This depends on the strength
# of your machine CPU. If you have a stronger machine, you might wanna set
# it to something like 12 seconds, if you have some kind of Xeon with less
# than 3.9Ghz, you might wanna set this to 15-20 seconds.
teleport-time: 15

# In how many seconds should we attempt to connect player to their
# sub-server after it being launched by /playerserver start command?
teleport-time-normal: 10

ram-limiting:
  # Should we use permissions for ram management? If set to true, you MUST give
  # your players permission playerserver.ram.<amount> (ex: playerserver.ram.512)
  # or, else, the command will be blocked, and player will not be able to create
  # the server. If set to false, everyone will have ram-per-server amount of RAM.
  use-permissions: false

  # How much RAM (in MB) should we allocate to each PlayerServer?
  ram-per-server: 512

player-limiting:
  # Should we use permissions for max-players management? If set to true, your
  # players should have playerserver.players.<amount>. The max amount of players
  # that you could give to a single server is 100000. You can also give them
  # playerserver.players.unlimited - for unlimited players. If the player
  # has no permission, he'll be able to have unlimited players.
  #
  # NOTE: If you use permissions, and you change player's permissions,
  # their server will need to reboot in order for changes to take place.
  use-permissions: false

  # What is the max players each server should have?
  max-players-per-server: 20

plugin-limiting:
  # Should we use permissions for max-plugins management? If set to true, your
  # players should have playerserver.plugins.<amount>. The max amount of plugins
  # that you could give to a single server is 20000. You can also give them
  # playerserver.plugins.unlimited - for unlimited plugins. If the player
  # has no permission, he'll be able to have unlimited players.
  #
  # NOTE: If you use permissions, and you change player's permissions,
  # their server will need to reboot in order for changes to take place.
  use-permissions: false

  # What is the max players each server should have?
  max-plugins-per-server: 20

# Should we enable permissions for server creation, deletion & more?
# If set to false, all the players will have access to those basic commands.
# Obviously, admin commands require permission no matter what.
enable-permissions: true
```



