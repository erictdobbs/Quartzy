Quartzy
===========                                       

Quartzy is a plugin for the Minecraft server API, Bukkit. It adds nether quartz ore to nether worlds that were generated before the 1.5 update.

Setup and Requirements
----------------------

Drop the quartzy.jar file into your server's plugin directory. Quartzy will create the configuration files on its first load. Quartzy has been tested with Bukkit release 2771.

Commands
--------

All commands require that the user either have operator permissions or give the command via server console. 

<dl>
  <dt>quartzy radius</dt>
  <dd>While in the nether, replace some netherrack with nether quartz ore in a square around you. Must be in the nether to use this command.</dd>
  <dt>quartzy x z radius</dt>
  <dd>Replace some netherrack with nether quartz ore in a square around nether coordinate (x,z).</dd>  
  <dt>quartzy delete radius</dt>
  <dd>While in the nether, replace all nether quartz ore with netherrack in a square around you. Must be in the nether to use this command.</dd>
  <dt>quartzy x z radius</dt>
  <dd>Replace all nether quartz ore with netherrack in a square around nether coordinate (x,z).</dd>  
</dl>

Configuration
-------------

Default config.yml file is created the first time the plugin is loaded through Bukkit. 

<dl>
  <dt>worldName</dt>
  <dd>Name of the directory holding the nether world regions files.</dd>
  <dt>genChance</dt>
  <dd>For every (x,z) coordinate in range, this is the chance that a quartz vein will be generated.</dd>
  <dt>radius</dt>
  <dd>The Manhattan distance radius of the generated veins.</dd>  
  <dt>density</dt>
  <dd>For every block within a vein, this is the chance that quartz will replace the existant netherrack.</dd>
</dl>