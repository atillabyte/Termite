# Termite

Termite decompiles, extracts, and assembles blocks, decorations, ids, and much more into a developer friendly format from Everybody Edits. This means that if your application that depends on blocks (such as a minimap generator) or another EE-related resource can be updated with new blocks almost instantaneously.

# Example

An example of the output is available at https://gist.github.com/Decagon/3bca5b7757016f9bd9f7 .


# How to use

## Termite

Download [freegame.swf](http://r.playerio.com/r/everybody-edits-su9rn58o40itdbnw69plyw/freegame.swf) from Everybody Edits and place the swf in the build directory (i.e the Debug folder or the Release folder.)

You have to have Java 8 Runtime or later installed (http://java.com/en/download/).

The app writes a JSON formatted array to the console, containing the following information about all blocks in the game:
- id
- layer (background or foreground)
- bmd (which system block package it is contained in, ex. decorations)
- the shop name
- description of the block (not many have these)
- item tab
- minimap color (in hexadecimal)
- block package
- the sprite offset in the respective image file (use bmd in conjunction with the consistent file-naming pattern to find the right image file.)

## PayVault Extractor

Simply choose the PayVault Extractor solution in the VS toolbar and start it. It will write all of the shop-related PayVault information in an easy-to-read, alphabetized file in YAML. The comments are generated from the shop descriptions. An example is available [here](https://github.com/Decagon/EEBlocks/blob/master/Other/payvault.yaml). 

# To Do
- ability to extract sprites from the image files using the sprite offset
