Real Recoil v1.2.1

The first-ever mod to bring proper recoil to the Mojave.

-----------
Description
-----------
- A dynamic, more realistic system with smooth camera movements and visible effort to control recoil
- Recoil values based on ammunition, for every type of ammunition in the game, with overall recoil also being inversely proportional to weapon weight and player strength
- An .INI file to edit recoil for any ammo type or add new ammunition types from mods (Optional CaliberX support and other mods already included)
- High compatibility with other mods
- Purpose-built for Hitman47101's incredibly well-made 1st Person Weapon Animation Overhaul (though it will work without it just as well)

Real Recoil brings a proper recoil system to Fallout: New Vegas. While there have been a number of recoil mods before Real Recoil, my aim is to make Real Recoil the best among them. Offering a dynamic set of mechanics, high compatibility, and very smooth visuals, Real Recoil offers the closest thing you'll find to recoil systems in modern shooters. Unlike previous recoil mods, Real Recoil, like most modern shooters, uses linear interpolation to calculate recoil for smooth movement, and has the player automatically compensate and fight to lower their weapon. 

In addition to this, Real Recoil bases recoil values on the type of ammunition a weapon is using, while also factoring in the weight of the weapon and player strength. Every type of ammunition in the vanilla game, it's DLC, and popular mods such as CaliberX, including variants of the same ammo (e.g. Standard vs +P), is given a recoil value appropriate to their real world counterparts. A lot of effort has been put into balancing these recoil values in a realistic way, but the included .INI file allows you to adjust, remove, or add new values to customize recoil (so yes, you can take away Energy Weapon recoil). This allows for high compatibility, with almost any downloaded weapon mod being immediately compatible with Real Recoil, and the ability to add recoil to any new ammunition added by a mod.

------------
Requirements
------------
 - New Vegas Script Extender (NVSE) - (http://nvse.silverlock.org/)
 - JIP NVSE Plugin - (http://www.nexusmods.com/newvegas/mods/58277/?)
 - Lutana NVSE Plugin - (http://www.nexusmods.com/newvegas/mods/55399/?)

----------------------- 
Highly Recommended Mods
-----------------------
While in no way required to run, it is highly recommended that you check out the mods listed here for maximum
enjoyment of Real Recoil. In particular, you should really check out Hitman47101's 1st Person Weapon Animation Overhaul
because it's fantastic and this mod was written, tested, and recorded (in the video above) with it active and in mind.
1. 1st Person Weapon Animation Overhaul - His optional Improved Iron Sights Fire Anims - Vanilla Pack which is also found in the downloads section of this mod is also highly recommended. 
	- (http://www.nexusmods.com/newvegas/mods/61501/?)
2. More Realistic Aiming - A fantastic mod which adds a very nice tremble separate from weapon sway to your aim. Believe it or not, it really enhances the experience.
	- (http://www.nexusmods.com/newvegas/mods/40652/?)
3. Project Nevada - What're the chances you don't have this anyway? But if you wanted the crosshair and dynamic weapon spread seen in the video above, Project Nevada adds that (and a whole lot more).
	- (http://www.nexusmods.com/newvegas/mods/40040/?)

------------
Installation
------------
1.  Mod Manager Installation
		If using a mod manager (I recommend Mod Organizer) simply download the latest version 
		via your mod manager.
2.	Manual Installation 
		Once downloaded, drag the contents of your the .zip file to your Data folder
		(on most systems, this will be C:\Program Files (x86)\Steam\SteamApps\common\Fallout New Vegas\Data).
		Start the New Vegas launcher and click "Data Files" and make sure "Real Recoil.esp" is checked off.
		
------------------------------------
How To Add/Remove/Change Ammo Values
------------------------------------
1. Navigate to the config folder (usually C:\Program Files (x86)\Steam\SteamApps\common\Fallout New Vegas\Data\Config)
2. Open up "Real Recoil.ini" in a text editor

-If Editing/Removing Ammo-
3. Use Ctrl+F to find the ammo in question, ommitting periods (e.g. "556mm" instead of "5.56mm")
4. Edit the value on the right side of the equals sign (If removing recoil, comment out or delete the line completely)
5. Save & Quit

-If Adding Ammo from a mod-
6. Create a new section in brackets with the name of the .esp or .esm that adds the ammo
7. Download and open FNV Edit (http://www.nexusmods.com/newvegas/mods/34703/?)
8. Find the ammo from the mod you want to add and lookup its FormID
9. Add its FormID to the new section ommitting the first two characters and any leading 0s (e.g. add "BCD8" instead of "0100BCD8")
10. Save & Quit

---------
Changelog
---------
Version 1.2.1
Bug Fixes
- Fixed an issue that caused recoil with grenades from Project Nevada and unsupported ammo

Version 1.2.0
New Features
- .INI system! Just a single .esp that works no matter what DLC or mods you have, and can be edited easily to change, add, or remove values instantly!
- Built-in support for CaliberX and other mods! Every ammo type in CaliberX now has a value. Feel the power of that 7.62x39mm!
- Additional support now for junk rounds added by Dead Money
Changes
- 12 Guage Beanbag lowered from 3.40 to 1.63
- .38 Special lowered from 1.56 to 1.17
- .45 and .45 HP increased from 1.68 to 1.96, +P from 1.82 to 2.16, and Super from 2.12 to 2.31
Bug Fixes
- Better performance (you likely won't notice it)

Version 1.1.0
New Features
- No longer locked to your frame rate, it now works in slow motion!
	- Fantastic for slo-mo in Project Nevada, or the slo-mo automatically initiated by the kill cam
	- Technical: Works through Delta timing, added by recalculating recoil via the kinematic equation, 
	  d = v*t + a/2*t^2 (well, just t^1 in the latter case for this instance to maintain greater parity with 1.0.0)
- Added a modifier to increase recoil for any pistol or gun held in a pistol fashion (i.e. both hands on the pistol grip)
Changes
- Decreased the "floatiness" of weapons
	- Technical: Increased the minimum speed of the rise before the player character begins compensating for recoil along with some other things
- Increased recoil value of .45 Super Ammo
Bug Fixes
- Changing ammo types or switching weapons no longer causes your weapon to recoil

Version 1.0.0
- First Release