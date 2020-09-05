---
description: >-
  Learn how to install and configure PlayerServers daemon and be the first to
  try out our experimental support for hosting your servers on multiple
  machines.
---

# Multi-Node Support

## Requirements

* Purchased PlayerServers. This addon if free of charge
* Have two \(or more\) machines
* Decent network connection
* At least 200MB of RAM dedicated to Daemon

## Instructions

The installation process for PlayerServers Daemon, even in developer beta is pretty straight forward. The first thing you need to do is simply enable multi-node support under experimental options at the end of your configuration file. After than, just reboot your BungeeCord and let the plugin generate required files.

After that's done, create a folder Daemon \(in /root directory, if possible\). Download the following jar file and drop it into your Daemon folder:

{% file src="../.gitbook/assets/daemon-v1.0-dev2.zip" caption="PlayerServersDaemon - BETA" %}

After that's done, run it for the first time by using `java -Xmx200M -jar (DaemonJarName).jar` in order to let it generate the required files. Now exit it by typing in `exit`. After that's done, configure both multinode.toml inside your BungeeCord/plugins/PlayerServers/multinode.toml and your Daemon config.toml which will be generated in your Daemon root directory.

As the last step, it is required to add a file named Spigot.jar \(any version from 1.8.8-1.16.1\) to your Daemon/templated directory and add all the wanted plugins to Daemon/plugins-to-be-added-ingame directory. If any of those directories were not created automatically, please create those manually. After that's done, please also copy PlayerServerCore.jar from BungeeCord/plugins/PlayerServers/templates/PlayerServerCore.jar to your Daemon/templates directory.

{% hint style="warning" %}
Great! You're done! Now, please note that PlayerServersDaemon is still under early-access development and may have a large amount of bugs. Please report all of those to our Issue tracker [here](https://gitlab.com/OpenSource02/playerservers/-/issues). Additionally, please take a backup of your MySQL Database and your server data before proceeding. We've taken every possible step to reduce the amount of possible issues that can happen, but we do highly encounter you to take those steps, just to be on the safe side.
{% endhint %}



