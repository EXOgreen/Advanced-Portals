---
sidebar_position: 1
description: Quick introduction to Advanced Portals.
---

# Tutorial Intro

1. Creating your teleport destination.
using the command `/destination create` or `/desti create` will create a new destination with the location data from your player (your player position and direction your facing).

2. Creating the portal blocks
Start by creating a frame for your portal, which can be any block you want, that we will then fill with the blocks that activate our portal. Using the command `/portal portalblock` gives you a wool block, that when placed turns into a nether portal frame. This allows you to create nether portal frames without commands. If the portal frames are facing the wrong way, hold the wool again and "break" (left click) the portal frames to rotate them.  Alternatively you can use `/portal endportalblock` or `/portal gatewayblock` to give you the other vanilla portal blocks, or even use water, lava, or other materials to act your portal trigger. 

3. Selecting the portal to create
After building your portal frame, we need to select the area that the portal encompasses. Use `/portal wand` to get an axe that allows you to select the area your portal will encompass. To use it, left click one corner of your portal to start selecting, and right click on the other corner to set bounding box.

4. Turning your selection into a working portal
The following commands are examples of how a portal can be created and used.

The command below makes a portal named WorldSpawn, to a previously created destination called spawn, that activates when a player touches a nether portal frame. 

`/portal create name:WorldSpawn destination:spawn triggerblock:NETHER_PORTAL`

and this command creates a portal named RandomTP, to a random location, that activates when a player touches water.

`/portal create name:RandomTP destination:spawn triggerblock:NETHER_PORTAL`

5. Teleporting players across servers
When using a mod such as BungeeCord, Waterfall, or Velocity, you can send players across servers. You will use the names from the configuration file for the proxy mod you are using. For example, if using Velocity, you would find your velocity.toml file on the velocity proxy server.

The command below makes a portal named SurvivalLogout, to a server called survival, that activates when a player touches a nether portal frame. When teleporting across servers and a destination is not specified, the default location is the last place you logged out. If it is your first time joining a server you will be sent to the world spawn.

`/portal create name:SurvivalLogout bungee:survival triggerblock:NETHER_PORTAL`

The command below sends you back to the hub world server, at a previously created destination called spawn.

`/portal create name:lobby bungee:lobby destination:spawn triggerblock:NETHER_PORTAL`

Here is a YouTube video made by [LtJim007](https://www.youtube.com/channel/UCZvGH5UFnZGHL7t11RLhg2w) explaining the basics.

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/nkOeMUkYz3Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
