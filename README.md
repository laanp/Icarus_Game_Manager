# Icarus Game Manager
An Excel Workbook and associated vba routines to manage various aspects of the game: Icarus-First Cohort

## Program Description

Welcome to the Icarus Game Manager!

This Excel Workbook and associated vba routines was originally developed as a project of mine to allow me to manage 
various aspects of the survival/building game - Icarus - First Cohort.

I have been playing the game for quite some time and when the developers released the Data Decentralization (Week #53 Update)
along with the Beta Dedicated Server app, I began messing with the local files on my PC to see what was possible, using 
my vba coding skills. 

The Icarus Game Manager is a collection of utilities and worksheets that allow the following in the game:

   - Icarus character information - Import, change, and export:
        - Character name
        - Character Experience Points (XP) - level
        - Talents and Rank - Unlock/Lock any
        - Tech Blueprints - Unlock/Lock any
 
   - Icarus Account information - Import, change, and export:
        - Change available currency: Ren, Exotics
        - Change available Talent Respec points
        - Loadout inventory - add/remove any Workshop item, including prefill/repair any item
        - Missions - Unlock/Lock any, and view mission duration & rewards info 
        - Workshop - Research/Unresearch any item

   - Modding - A modding component for the game, including:
       - Unpack Icarus game (*.json) files
       - Support for customized scripting language to make changes to game (*.json) files
       - Unpack/Repack mod files (*.pak)
       - File management between customized mods folder & the Icarus mod folder location
                     
   - Dedicated Server:
       - Allows management of an Icarus Dedicated Server, including:
       - Query and Update Icarus Dedicated Server app through SteamCMD
       - Start/Stop Icarus Dedicated Server
       - Manage Dedicated Server startup parameters
       - File management for mods between customized mods folder/Icarus mod folder to Dedicated Server mods folder
       - File management for Prospects between local Icarus client prospects folder to/from Dedicated Server prospects folder
               
   - Fish Information:
       - Allows reading fish information from game files, including what map, what region, and what lure to catch them!

   - Resource Information:
       - Allows quick search & lookup of local database for Icarus resource information.
       - Answers the questions: "What is this used for?" and "Where can I craft it?" and "What do I need to craft it?" 


# Requirements

The Icarus Game Manager is a Microsoft Office 365 Excel macro-enabled workbook and requires you to have the latest version of Excel.

It might work on older versions of Excel, but it hasn't been written to support them.
 
Ensure macros are enabled in Excel, and this workbook is Trusted in macro security settings. To set the Trust Settings in Excel:
-  In Excel, select File...Options...Trust Centre...Trust Center Settings...Trusted Locations... add a new folder location to this list
   (where you keep the Icarus Game Manager) & select checkbox (Subfolders of this location also trusted)... click ok.

Some routines in this workbook make directories, add/delete/move files, so ensure your Anti-virus software allows this workbook access.


# Download/Installation Instructions

   - Download file: "Icarus_Game_Manager.zip" from github - Unzip into any directory on your PC, maintaining folder structure

   - Download file: "UE4_Icarus_Unrealpack.zip" - Unzip into any directory on your PC, maintaining folder structure
       - Only required if you want to utilize modding utilities in this workbook, or want to look at latest Fish Data.

   - Download the Steam Console Client - SteamCMD: https://steamcdn-a.akamaihd.net/client/installer/steamcmd.zip
       - Only required if you are setting up an Icarus Dedicated Server and want to run the server utilities in this workbook.
       - Read the "Setting Up A Local Dedicated Icarus Server.txt" on downloading/installing steamcmd and setting your local Dedicated
         Icarus Server.  I highly recommend this step, as you will realize a higher graphics framerate running a dedicated Icarus server
         on your machine, and connect to it over LAN with your local Icarus game client.  Plus it's a great way to have 2 copies of all 
         your prospects (missions, open worlds and outposts) as Dedicated Icarus Server prospects and local Icarus prospects 
         reside in different folders. 


# Setup Instructions

After you have downloaded and installed the neccessary files, you can startup the workbook "Icarus - Game Manager (vXX_wYY).xlms"
The first sheet that will come up is the "Home" sheet, which will identify the current workbook version, and the last revision
of the Icarus game files when this workbook was released.

This "Home" sheet requires all the directory locations to be set, as per the instructions on the sheet.  After all the locations have been
set, click the "Check Directories" button at the top of the page to verify all directories are good.  
 

# Navigating the Menu

At all times, you will see a ribbon menu item next to the "File" menu, called "Icarus".  This is the menu entry point to access all the utilities in this
workbook.  At all times, the "Setup", "Sheet Views" and "Help" group of buttons will be visible, and depending on which "Sheet View" button 
you have selected, there will be additional context-specific menu groups/buttons as well as worksheets made visible.

The "Help" button is specific to the current Sheet View context at all times, and a good source of information for the buttons and sheet
views that are displayed.  Hovering your mouse over any button will provide pop-up context-sensitive help messages, for what the button does.
If you do not see the pop-up context-sensitive help messages when you hover the mouse over the button, change the following options in Excel:
    - Goto "File..." "Options..." "General..." under the "User Interface Options" section, set the "Screentip Style" dropdown box
      to "Show feature descriptions in ScreenTips".


  