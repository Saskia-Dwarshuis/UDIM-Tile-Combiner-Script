# UDIM Tile Combiner Script for Substance Painter and Photoshop

**UDIM Tile Combiner Script for Substance Painter and Photoshop** is a Photoshop script built for combining UDIM tile texture maps split across multiple images into one map (on a per-UDIM-number by per-material-channel basis.)

## Disclaimer

This script was written and tested on only a Windows computer. I have done my best to make the script work for MacOS, but there may be issues. Likewise only installation instructions for Windows are listed, but MacOS shouldn’t be much different.

The script was only tested on Photoshop CC versions 2019 and 2020. Backwards and forwards compatibility is likely, but not guaranteed.

## Installation Instructions

### Windows

#### If you have administrator permissions:
1. Download the most recent release.
2. Unzip the release file and place *UDIM Tile Combiner.jsxbin* and the *UDIM Tile Combiner Script for Photoshop Library Scripts Only* folder in the Photoshop scripts folder. *README.md* can be deleted.
3. Edit the permissions of the *UDIM Tile Combiner Script for Photoshop Library Scripts Only* folder— for Users, give the permission to write. This is to enable the active settings data and the previous session data to be written in their appropriate files.  
4. Open Photoshop and browse to File > Scripts. *UDIM Tile Combiner* should show up as a script available to run.

#### If you don’t have administrator permissions:
1. Download the most recent release
2. Locate a place on your computer where you can easily access/navigate to and where administrator permissions are not required. Unzip the release file and place *UDIM Tile Combiner.jsxbin* and the *UDIM Tile Combiner Script for Photoshop Library Scripts Only* folder at this location. *README.md* can be deleted.
4. Open Photoshop and browse to File > Scripts > Browse. Navigate to the place where you put *UDIM Tile Combiner.jsxbin* and load the script. You will have to repeat this step each time you want to run the script.

## How To Use

### Substance Painter Export Settings

* Add an alpha channel to each material channel exported, with *Opacity* or *2D View* used as the alpha value. 
* *Dilation + Transparency*, with a low dilation value. 

### Combiner Script Walkthrough

![UDIM_Tile_Combiner_UI_Numbered](https://user-images.githubusercontent.com/83183389/116453204-98c4e500-a82c-11eb-98db-66bf6a7f3e97.png)

1. Select a source folder, which should contain the texture maps exported from Substance Painter. 
2. Select a destination folder, into which the combined images will be saved.
3. Choose which tile setting the script should work with when combining texture maps and change the UDIM tile number values if necessary. 
4. Add or remove material channel sort terms the script should work with when combining texture maps. 
5. Change or remove the combined texture maps’ save name prefix (the default is “Prefix_”).
6. Select which file type to save the combined texture maps as (the default is .png).
7. Run the script!

### Other Features

#### Tile Combiner Settings to Load

Default radio button— If selected, loads in the script settings saved in *UDIM Tile Combiner Script for Photoshop Library Scripts Only/DefaultSettings.js*.

Previous Session radio button— If selected, loads in the script settings saved in *UDIM Tile Combiner Script for Photoshop Library Scripts Only/PreviousSessionSettings.js*. *PreviousSessionSettings.js* is written to at the end of each complete script run, saving the script settings used.

User Defined Preferences radio button— If selected, loads in the script settings from whatever file the load button is pointing to (the default is *UDIM Tile Combiner Script for Photoshop Library Scripts Only/UserSetSettings.js*).

Set button— Takes a snapshot of the current script settings and creates a new settings file with that information. The user selects what folder to save that file in, and what name the file should have (but the file type will always be .js). The script will automatically set this new file as the user set setting file to reference if the User Defined Preferences radio button is clicked. 

Load button— Opens a file selection dialog to allow the user to select a user set settings file. The settings saved within that file will then update the current script settings, and will update the script with those settings each time the User Defined Preferences radio button is clicked. The selected settings file will remain the file that gets referenced for the User Defined Preferences radio button until another file is selected, as the selected settings file path gets written to *ActiveSettings.js* at the end of every script run and then gets referenced at the beginning of each instance of the script thereafter. 

Reset Current Folder Paths button— Any source folder selected and any destination folder selected will be reset to no entry. 

#### Other Script Settings

Folder selection shortcut mode checkbox— If enabled, the second folder selection dialog (the destination folder, typically) will open with the file path of the first folder selection (the source folder, typically). If disabled, the folder selection dialog will always open at the desktop. 

“Script completed!” alert checkbox— If enabled, an alert will run at the end of the combining process. 

Ignore image overwriting warnings checkbox— If enabled, the combining script will ignore any image overwrite warnings. If disabled, an alert will sound for each image overwritten, requiring the user to allow or skip the overwrite. 
