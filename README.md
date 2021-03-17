# brawllib-wit

A collection of command-line interfaces to [BrawlLib](https://github.com/soopercool101/BrawlCrate) that can be helpful in Wii Virtual Console injection.

## bannercfgfromtxt

Reads the given banner.cfg.txt file and replaces each field with the contents of a text file in the current directory with the same name as the field.
For example, the Japanese name will be replaced with the contents of JP.txt (if it exists, otherwise the existing title is kept).

Usage: `bannercfgfromtxt.exe path/to/banner.cfg.txt`

## imgoverlay

Overlays one image onto another at a certain position and writes the output to a third file.

Usage: `imgoverlay.exe larger.png smaller.png x y width height output.png`

## openingimet

Finds the game's name (in the given language) in the opening.bnr or 000000000.app file, and prints it to the console.

Usage: `openingimet.exe 000000000.app [ja|en|de|fr|es|it|nl|7|8|ko]`

## openingimet

Decompressed and extracts one of the three .arc files from the 00000000.app.

Usage: `openingextract.exe 000000000.app [banner|icon|sound] output.arc`

## texextract

Extracts a single TEX0 or TPL texture to an image file.

Usage: `texextract.exe input_file.tex0 output_file.png`

## texreplace

Replaces a single TEX0 or TPL texture with an image from another file.

Usage: `texreplace.exe file_to_modify.tex0 replacement_file.png`

## u8pack

Creates a U8 archive that includes all files in the current directory.

Usage: `u8pack.exe output.arc`

## u8unpack

Extracts all files and folders in a U8 archive to the current directory.

Usage: `u8unpack.exe input.arc`

## wteconvert

Converts RGB5A3 data between .wte and .tex0 formats.

Usage: `wteconvert.exe file.[wte|tex0] out.[wte|tex0]`
