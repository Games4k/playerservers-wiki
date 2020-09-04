---
description: Below is the list of all the commands & plugin permissions
---

# Permissions & Commands

## Commands

<table>
  <thead>
    <tr>
      <th style="text-align:left">Command</th>
      <th style="text-align:left">Aliases</th>
      <th style="text-align:left">Plugin</th>
      <th style="text-align:left">Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">/playerserver</td>
      <td style="text-align:left">/ps</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">Gives you the plugin description &amp; licence info.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>create</p>
      </td>
      <td style="text-align:left">none</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">Creates a new subserver if you don&apos;t already
        <br />have one.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>start</p>
      </td>
      <td style="text-align:left">
        <p>/ps boot</p>
        <p>/ps enable</p>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">If your server is offline, it will try to boot it up.</td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>delete</p>
      </td>
      <td style="text-align:left">/ps remove</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>At first it asks you to confirm your decesion by</p>
        <p>repeating the command, tha it removes your</p>
        <p>sub-server and removes you from the database.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>reboot</p>
      </td>
      <td style="text-align:left">/ps restart</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Gives you some info on how to restart your</p>
        <p>sub-server.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>stop</p>
      </td>
      <td style="text-align:left">
        <p>/ps shutdown</p>
        <p>/ps forcestop</p>
        <p>/ps disable</p>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Forcefully kills your sub-server. Not</p>
        <p>recommended at all and can cause some</p>
        <p>world destruction. Chunks could be damaged.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>join</p>
      </td>
      <td style="text-align:left">/ps connect</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Connects you to your sub-server and gives</p>
        <p>you your ServerID and a special command that</p>
        <p>your friends can use to connect to your server.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>admin delete</p>
      </td>
      <td style="text-align:left">none</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Followed by serverID, forcefully kills and</p>
        <p>removes the server with given serverID.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>/playerserver</p>
        <p>admin update</p>
      </td>
      <td style="text-align:left">none</td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Automatically download and update</p>
        <p>PlayerServerCore accross all of your Player</p>
        <p>servers. Note that this will require manual</p>
        <p>restart of each subserver, in order to take effect</p>
      </td>
    </tr>
  </tbody>
</table>

## Permissions

I know, there are not much permissions, but that's just to keep things simple. Yes, I could make one permission for every single command, but I just don't see the real usage for such a thing like that.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Permission</th>
      <th style="text-align:left">Plugin</th>
      <th style="text-align:left">Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left"><b>playerserver.manage</b>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>This permission node allows the player to create,
          <br />manage, and delete their sub-server. It will only work if</p>
        <p><code>enable-permissions</code> is set to true in the config file.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>playerserver.admin</b>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>This permission node allows the player to execute</p>
        <p>admin commands, such as /playerserver admin delete.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left"><b>playerserver.menu</b>
      </td>
      <td style="text-align:left">PlayerServers Hub</td>
      <td style="text-align:left">
        <p>This permission allows the player to execute <code>/pslist</code>
        </p>
        <p>or <code>/serverlist</code> command.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>playerserver.players.</p>
        <p>&lt;amount&gt;</p>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Limits the amount of players that player&apos;s server can</p>
        <p>have. You can do playerserver.players.unlimited too.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>playerserver.ram.</p>
        <p>&lt;amount&gt;</p>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Amount of RAM in MB that player&apos;s server will be</p>
        <p>started with. <b>The max amount you can set is 20000</b>.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">
        <p>playerserver.plugins.</p>
        <p>&lt;amount&gt;</p>
      </td>
      <td style="text-align:left">PlayerServers Bungee</td>
      <td style="text-align:left">
        <p>Limits the amount of plugins that player can install.</p>
        <p>You can do playerserver.plugins.unlimited too.</p>
      </td>
    </tr>
  </tbody>
</table>

