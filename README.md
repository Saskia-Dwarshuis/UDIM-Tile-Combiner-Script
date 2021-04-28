# UDIM Tile Combiner Script for Substance Painter and Photoshop

**UDIM Tile Combiner Script for Substance Painter and Photoshop** is a Photoshop script built for combining UDIM tile texture maps split across multiple images into one map (on a per-UDIM-number by per-material-channel basis.)

## Disclaimer

This script was written and tested on only a Windows computer. I have done my best to make the script work for MacOS, but there may be issues. Likewise only installation instructions for Windows are listed, but MacOS shouldn’t be much different.

The script was only tested on Photoshop CC versions 2019 and 2020. Backwards and forwards compatibility is likely, but not guaranteed

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

### Substance Painter Export Settings

// Export settings
### Combiner Script Walkthrough

1. Select a source folder, which should contain the texture maps exported from Substance Painter. 
2. Select a destination folder, in which the combined images will be saved to.
3. Choose which tile setting the script should work with when combining texture maps and change the UDIM tile number values if need be. 
4. Add or remove material channel sort terms the script should work with when combining texture maps. 
5. Change or remove the combined image save name prefix (the default is “Prefix_”).
6. Select which file type to save the combined images as (the default is .png).
7. Run the script!

### Other Features

#### Tile Combiner Settings to Load

// Explanation of section

#### Other Script Settings

*Folder selection shortcut mode* checkbox— If enabled, the second folder selection dialog (the destination folder, typically) will open with the file path of the first folder selection (the source folder, typically). If disabled, the folder selection dialog will always open at the desktop. 

*“Script completed!” alert* checkbox— If enabled, an alert will run at the end of the combining process. 

*Ignore image overwriting warnings* checkbox— If enabled, the combining script will ignore any image overwrite warnings. If disabled, an alert will sound for each image overwritten, requiring the user to allow or skip the overwrite. 
