HecticHotBar script for Tes3MP 0.7-Alpha  
Author: HecticKaluha  
Date: 13/01/2022  


# HecticHotBar
A Tes3MP server side script to enable a customizable "hotbar" in the chatwindow that displays the player's quickkeys. No more need to memorize all those items and spells!


## INSTALLATION:
1) Save the script `HecticHotBar.lua` to your `tes3mp-server\server\scripts\custom` folder as `HecticHotBar.lua`.
2) Open `customScripts.lua` in a text editor such as notepad. It can be found in your `tes3mp-server\server\scripts` folder.
3) On a new line, add the following: `require("custom.HecticHotBar")`
4) Make sure there are no dashes infront of it. (Dashes infront will disable/comment it out.)
5) Save `customScripts.lua`, restart your server, and enjoy.

### Configuring and customizing
After you installed the script following the steps above, you may want to customize the hotbarsettings or the command. To do this follow the steps below:
1) Run the server once with the script enabled. Doing this will generate the config file. The config file will be located at `tes3mp-server\server\data\custom\__config_HecticHotBar.json`.
2) Stop the server.
3) Open the config file that was created in step 1 and edit the values under `settings` as you like.
- **NOTE** If you want to add support for items or spells from other mods, you can add the refId of these items followed by the name they should have under `customItems` in this config file. You can follow the example code in the file if you don't know how to. *If you don't do this the script will still work and just display the refId of the item instead, which in most cases is still quite readable.* 
4) Save and close the file. 
5) Start the server. The script will now use your custom config setting.


## DESCRIPTION:
This Tes3MP serverside script enables a nifty "hotbar" that is displayed in the chatwindow of Tes3MP.
The scripts adds a new command for the players to use, namely "/hotbar" (this command can be changed to whatever you desire through the configfile). This command will generate a text based hotbar in the chatwindow for the hotkeys of the player that executed the command. 
**The chatwindow can be resized and dragged to the desired position to look and feel more like an actual hotbar/actionbar.** 
The script works with ALL base game items and ALL custom items created through alchemy, enchanting or spellmaking. 
If you're using addons that add extra items, spells or equipment, the script allows you to add support for these custom items through the config file.
If you don't add support for these items, the script will still work and will just display the refId of the item instead, which in most cases is still quite readable. 


## FEATURES:
- A clean looking textbased hotbar based on the players current custom quickkeys (F1 quickkeys menu)
- The hotbar shows the name of in-game items (base armor, books, clothing, enchanted items, miscellaneous items, potions. spells and weapons)
- The hotbar shows the custom names given to items (from enchanting or alchemy for example) like armor, books, clothing, enchanted items, miscellaneous items, potions. spells and weapons
- The hotbar takes possible empty quickkey slots into account and shows that these slots are empty in the hotbar too.
- The hotbar autoupdates when you change quickkeys. No need to retype the command. This way you always have an up to date Hotbar for those clutch encounters or roleplay scenarios.
- A config file to adjust setting of the hotbar to your liking i.e. the command used, autoupdate setting, hotbar colors for the slotnumber, item or spellname, and the deviderlines
- Support for custom items added through other mods like Tamriel Rebuilt for example.

## IMAGES:
The hotbar in-game.
![The hotbar ingame](https://user-images.githubusercontent.com/11851645/149352570-4d132541-edd6-47d9-a5e1-bf1692bdd974.png)

The hotbar in-game with the quickkeys for reference
![The hotbar in-game ](https://user-images.githubusercontent.com/11851645/149352732-ea6ffdca-22ba-4175-8b04-e739392a200c.png)
