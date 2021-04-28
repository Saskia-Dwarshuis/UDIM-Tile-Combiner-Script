# UDIM Tile Combiner Script for Substance Painter and Photoshop

**UDIM Tile Combiner Script for Substance Painter and Photoshop** is a Photoshop script built for combining UDIM tile texture maps split across multiple images into one map (on a per-UDIM-number by per-material-channel basis.)

## Disclaimer

This script was written and tested on only a Windows computer. I have done my best to make the script work for MacOS, but there may be issues.

The script was only tested on Photoshop CC versions 2019 and 2020, but it should work on Photoshop versions reaching back to CS6, if not further— however, this is not ensured.

## Installation Instructions

### Windows

#### If you have administrator permissions:
1. Download the most recent release
2. Unzip the release file and place *UDIM Tile Combiner.jsxbin* and the *UDIM Tile Combiner Script for Photoshop Library Scripts Only* folder in the Photoshop scripts folder. *README.md* can be deleted.
3. Edit the permissions of the *UDIM Tile Combiner Script for Photoshop Library Scripts Only* folder— for Users, give the permission to write. This is to enable the active settings data and the previous session data to be written in their appropriate files.  
4. Open Photoshop and browse to File > Scripts. *UDIM Tile Combiner* should show up as a script available to run.

#### If you don’t have administrator permissions:
1. Download the most recent release
2. Locate a place on your computer where you can easily access/navigate to and where administrator permissions are not required. Unzip the release file and place *UDIM Tile Combiner.jsxbin* and the *UDIM Tile Combiner Script for Photoshop Library Scripts Only* folder at this location. *README.md* can be deleted.
4. Open Photoshop and browse to File > Scripts > Browse. Navigate to the place where you put *UDIM Tile Combiner.jsxbin* and load the script. You will have to repeat this step each time you want to run the script.

## How To Use

### Overview

// From Substance Painter settings

1. Select a source folder, which should contain the texture maps exported from Substance Painter. 
2. Select a destination folder, in which the combined images will be saved to.
3. Choose which tile setting the script should work with when combining texture maps and change the UDIM tile number values if need be. 
4. Add or remove material channel sort terms the script should work with when combining texture maps. 
5. Change or remove the combined image save name prefix (the default is “Prefix_”).
6. Select which file type to save the combined images as (the default is .png).
7. Run the script!

### Other features

#### Tile Combiner Settings to Load

// Explanation of section

#### Other Script Settings

*Folder selection shortcut mode* checkbox—

*“Script completed!” alert* checkbox—

*Ignore image overwriting warnings* checkbox—
