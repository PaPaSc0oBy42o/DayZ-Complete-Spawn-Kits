You can add all the corresponding loadout JSON files to the custom folders on your local PC, Xbox, and PS servers.

First things first is to ensure you have cfggameplayfile.json enabled. To do so, clcik on your "General" tab under settings on your Web Interface. Scroll down and select "enable cfggameplay.json".

Next click on the "File Browser" tab on your W.I and follow this path: dayzstandalone/mpmissions/dayzOffline.chernarusplus, download your "cfggameplay.json" file (make a backup) and open it in a text editor. (I recommend Notepad++)

In your cfgameplay file edit the string of line from this:

"PlayerData":
	{
		"disablePersonalLight": false,
		"StaminaData":

To this:

"PlayerData":
	{
		"disablePersonalLight": false,
		"spawnGearPresetFiles": ["custom/m4a1_loadout.json","custom/SVD_loadout.json","custom/aug_loadout.json","custom/DMR_loadout.json"],
		"StaminaData":

This is where your server gets permission to use the custom files. (The example provided is using the original files names - they can be edited to whatever you decide to name the files. Just make sure to edit the cfggameplay file name if you change the loadouts name.)

From here all you have to do is upload the individual ffles to the customs folder and start/restart your server. 

You can access the custom folder on your server by going first going to "File Browser" on your servers web interface.
Follow the provided path to access the customs folder on your server: dayzstandalone/mpmissions/dayzOffline.chernarusplus/custom. (If you don't have a customs folder, make a new directory named custom)(dayOffline.enoch for Livonia map)
Select "Upload file
