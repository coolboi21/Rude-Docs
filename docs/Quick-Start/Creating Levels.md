# Creating Levels

Standard objects
You will need several standard objects in your level. These can be copied from the essentials level in Custom/essentials.unity, or the essentials scene can be copied as a template

EventSystem
BeamDirectionSetter
Level Info: This object contains the text for the level name popup when the door opens. Under Assets, there are two fields called Large Image and Large Text. Large Image is used to detect the level preview image in menu, but also used to detect which level player is in. You may see discord rich presence icon change according to this value. Large text is used as the title for the stats tab (when you press tab)
StatsManager: Contains values for maximum time, minimum kills and minimum style for ranks. Time is measured in seconds. If time ranks are set to [60, 90, 120, 150], S rank requires max 60 seconds, A rank requires max 90 seconds etc.
StatsManager/MusicManager: Contains the calm/battle/boss audio sources as children. If you want ambient sound at the beginning of the level (for example 6-1) you can make an audio source for the ambient and disable the music manager until it is needed.
OutOfBounds: Kills enemies and teleports the player back
FirstRoom: This room is where the player spawns. This room must have the default position of (0, 0, 300). You should NOT use the original prefab. Instead, use the rude's dummy prefab which is replaced with the original one in the game. Several settings can be changed from here as well such as background color, skybox, music/title display on door open.

https://www.youtube.com/watch?v=6PHrCwGiavU

---
*Guide Written By: LUKA*
