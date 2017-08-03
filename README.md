# Kagerou Settings
My settings for the kagerou overlay for ACT

## Pre-requisits
1. Go to the [ACT Page](http://advancedcombattracker.com/) and download the advanced combat tracker
2. Download the [FFXIV Plugin](http://advancedcombattracker.com/includes/page-download.php?id=66)
3. Open the Windows Firewall application (This is for Windows 10)
    1. Click on "Allow an app or feature through Windows Firewall"
    2. Click on "Change Settings"
    3. Click on "Allow another app..."
    4. Click on "Browse..."
        1. Navigate to where you installed ACT (This is usually in C:\Program Files (x86)\Advanced Combat Tracker)
        2. Enable "Advanced Combat Tracker.exe"
    5. Check the Private setting as well as the Public setting for ACT
    6. Click "OK"
    7. Exit Firewall and restart (preferably your computer)
4. Remove the FFXIV Overlay (Top right in ACT)
5. Go to Options
    1. Main Table/Encounters -> General
        1. Change "Number of seconds to wait after the last combat action to begin a new counter." to 30
    2. Output Display -> Text Export Settings
        1. Click on add preset in the top right
        2. Click on "Edit Directly" under "Allies Formatting" and paste the following
            1. `({duration}) {title}: {ENCDPS} | {maxhit}`
            2. Press Save
        3. Click on "Edit Directly" under "Per-combat Formatting" and paste the following
            1. ` | {NAME5} -> {ENCDPS}`
            2. Press Save
        4. Click "Add Text Format Preset"
        5. Change the "Clipboard Formatting" option to the newly created setting which will be as below
            1. `(EncDPS) " | {NAME5} -> {ENCDPS}`
6. Go to Plugins
    1. Click "Browse..."
    2. Find the dll file that you downloaded as the FFXIV Plugin (it'll be FFXIV_ACT_Plugin.dll as default)
    3. Click on Add/Enable Plugin
    4. Go to FFXIV Settings
        1. Go to Parse Options and check Combine Pets with Owner
7. You should now be able to see your damage automatically updating in the Main window

## Installing the Overlay
1. Download the [Overlay Plugin](https://github.com/hibiyasleep/OverlayPlugin/releases/tag/0.3.3.11)
3. Download the zip file from here at the top of the page http://billyvg.github.io/OverlayPlugin-themes/
2. Right click both zip files, click on properties, then check "Unblock" and apply
3. Add it to ACT then navigate to it in the plugins page
4. Click on the mini parse and click on the triple dot next to the url box, and navigate to the extracted overlay plugin themes directory, and select the html file that you like, I'd recommend the Hibiyasleep Kagerou pointer as there's an export that's handy for stormblood below
5. Input some settings as you wish, recommended settings are below:
    1. Click on the three vertical dots on the top right hand of the overlay
    2. Click on the cog
    3. Click on the first dropdown you see on the right hand side, change the overlay to english
    4. Click on the button in the top right of the settings to save
    5. (Optional) Go to Import/Export and paste in the code from the [export](export.txt) file and click on import

***Always remember to start ACT as administrator!***
