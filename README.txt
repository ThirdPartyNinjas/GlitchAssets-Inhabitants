GlitchAssets-Inhabitants
==============================================================================
This is a straight-forward conversion of the flash assets files from the game Glitch, which were released into the public domain. I performed the conversion at 2x original scale.

See http://www.glitchthegame.com/public-domain-game-art/ for more information.

The repository contains only the Inhabitants.

Conversion process:  
I wrote three scripts that run inside of Flash (I used Adobe Flash Professional CC).
After running the scripts, the output folder was enormous because there were a lot of duplicate images. I ran VisiPics to look for duplicates and delete them.

RecursiveExportFile - Recursively searches through folders looking for *.fla files, and calls exportPNG on them. This works well for basic files, but if there's any animation, it will be lost.

RecursiveExportPieces - This one searches through each flash file for individual components, exports those individually. Movie clips are exported as png sequences. This one will dump everything out, sometimes getting way too much data.

RecursiveExportPiecesFlat - Same as "Pieces" but it doesn't export sequences. This means some data will be lost, but it's a better choice for some of the data. I decided experimentally which one was better.
