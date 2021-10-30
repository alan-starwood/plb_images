readme.txt for ballcaps folder
------------------------------

Ballcap texture
---------------

Whenever a ballcap is "painted" for the first time after loading the database, the game creates a texture for the baseball caps of that team. The textures are based on the file baseball_cap_base.png, which you can find in the folder /data/facegen. Don't change that file!

If you want to create customized textures for certain teams, do the following:

- locate the folder /data/ballcaps
- copy the file default_ballcap_texture.png which you can find in that folder
- rename the copy to caps_ + team name + underline + team nickname + .png
Remove all dots in the team name and nickname, and replace all spaces with underlines.
- edit the file as you like.

This file will then be used "globally" for each team with that name and nickname, for any new database.
There is a folder /ballcaps in each database folder, too. To define a ballcap texture for a team on database level, you place the file in that folder.

When the game looks for a texture, it will first look in the database folder and use a file if it exists. If there is no file, it will look into the "global" folder /data/ballcaps. If there is a file, it will be copied into the database folder and used from there in the future!

If no file is found at all, OOTP will load the file /data/facegen/baseball_cap_base.png and "paint" the texture using the team colors.

The 5 five segments are used as followed:
1. top left: the lower side of the visor
2. below that the front part of the cap
3. right of that the upper side of the visor
4. the two parts at the bottom are the right and left side of the cap, which together also form the back of the cap
5. the circle is the knob on top of the cap

Secondary team logo
-------------------

If there is a file named caps_logo_ + team name + underline + team nickname + .png (remove all dots in the team name and nickname, and replace all spaces with underlines) in the folder /ballcaps, it will be used as the logo for the caps!

Individual colors
-----------------

You can define a color for the cap and another (or the same) color for the visor in the team settings in the game. You can also add the color information to the caps logo file. Just add the 6 character HTML color codes of the main color and of the visor color like this:
logo_teamname_nickname_FFFFFF_000000_sometext.png
"sometext" is optional and can be any text, like your name or the name of the logo set or whatever.
FFFFFF will be the color of the ballcap. It's the color code for white color.
000000 will be the color of the visor. It's the color code for black color.

