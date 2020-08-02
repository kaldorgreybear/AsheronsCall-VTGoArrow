# GoArrow-VVSEdition
Forked GoArrow from Virindi SVN repo

To get the compiled dll, go to https://www.arcayn.com/asherons-call/goarrow-update-with-working-dungeon-maps/

This version changes the way the maps are stored locally a little.  The version I originally downloaded to play retro Asheron's Call didn't load up the maps correctly and no "hacks" or fixes would make it work.  I was able to track down the old dungeon maps and dungeons.txt, so instead of worrying about more internet sleuthing to find the CSV file, I just changed this version to pull the file it really needs in the end, dungeons.txt, from the server instead.

The changes are in 2 files, DungeonHud.cs and settings.settings.  There are a few new settings added to control the lenght of time things are cached and repulled, and a new setting for the location of the web version of dungeons.txt to download.

The plugin has some trouble downloading the dungeons.txt and working on a clean load, so for now there is some output logging in place that will notify that the file was downloaded and to reopen to see dungeon maps with GoArrow.

These maps download from arcayn.com archive.

To install download the two files under releases, the DLL and dll.config.
Copy to your goarrow folder, default is C:\Games\VirindiPlugins\GoArrowVVSEdition
Click yes to overwrite the two files
Restart AC if it's already open. 
