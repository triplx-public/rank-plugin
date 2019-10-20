<h1>TriplX Ranking</h1>
The rank plugin for TriplX

This document record the functionality of this plugin, and covers what it does and does not do in the full network overview.


<h2>What this plugin is</h2>
This plugin manages ranks and permissions of players on all servers. The plugin goes in all servers, and edits and keeps track of player ranks.

<h2>Functionality</h2>
**The plugin covers the followning**:

 - Prefixes on player join (chat AND tablist)
 - Editing player ranks (command)
 - Updating MongoDB for all new ranks
 - Auto tracks rank updates
 - Manages chat formatting
 
 
**Does not cover**:

 - Nickname prefixes (/nick is not taken into consideration- yet)
 


<h2<Details</h2>
The details of the plugin (commands, events)

<h3>Commands</h3>
**/rank** 
  <set> <player> <rank> - Change a player's rank to a new one.
  <history> <player> - Access the rank history of a player.
  <revert> <player> - Change a player's rank to the one they have previously.
    

<h3>Listeners (Events)</h3>
**Player Chat Event**
  It utilizes the player chat event to set the chat format and apply the user's prefix. 
  
**Player Join**
  It watches for when player joins so that the prefix can be applied in tab, 
  and if necessary update data in mongo (if new player, or there was a name change)
    
  

    


