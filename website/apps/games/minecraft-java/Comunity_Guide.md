# Minecraft Java Community Guide

⚠️ **Warning This guide contains information that uses Advanced/Expert settings. As a result this will be outside the scope of support!** ⚠️

# Running Multiple MC-Java Servers

You can easily run Multiple MC Servers. You simply need to change the external ports, Be sure to use an unused port. There is no need to change the Minecraft port or RCON port in the server.properties

MC Server 1

<div>
<a href="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-server1.png"><img src="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-server1.png" width="100%"/></a>
</div>

MC Server 2

<div>
<a href="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-server2.png"><img src="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-server2.png" width="100%"/></a>
</div>

# Plugins DIR

To easily get Plugins in to your MC server since PVC&#39;s are in use for the config storage you can add a host path storage for either /mods or /plugins depending on what your server needs like so

<div>
<a href="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-plugins.png"><img src="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-plugins.png" width="100%"/></a>
</div>

This will give you an easy folder to drop the plugins in and they will then sync to /data/plugins or /data/mods , you will/may need to shell in to the app to periodically clean up old versions

# Plugins/mods that need additional ports

Using Dynmap as an example Under network and Services Check Show Expert config (remember the warning at the top?)

Click Configure add Manual Custom Services and fill out like so also adding Configure additional service ports

<div>
<a href="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-modports1.png"><img src="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-modports1.png" width="100%"/></a>
</div>

For the second server instance the setup is about the same one minor difference is the need to change the port for dynmap in the container to a new port and configure like so (note this could of just been my system being silly due to my tests and not rebooting)

<div>
<a href="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-modports2.png"><img src="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/mc-modports2.png" width="100%"/></a>
</div>

Dynmap Web working

<div>
<a href="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/dynmap.png"><img src="https://truecharts.org/_static/img/communityguide/apps/games/minecraft-java/dynmap.png" width="100%"/></a>
</div>
