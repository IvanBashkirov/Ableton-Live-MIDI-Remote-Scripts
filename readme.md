This is a Control Surface script for Nektar Pacer that allows tight intergration with Ableton Live (tested with version 9.7 only). The mapping is as follows:

| Switch | Function                                   |
|--------|--------------------------------------------|
| A      | Enable/disable currently selected track    |
| B      | Solo currently selected track              |
| C      | Next scene                                 |
| D      | Previous scene                             |
| 1      | Session Record Button                      |
| 2      | Previous Track                             |
| 3      | Next Track                                 |
| 4      | Stop all clips on currently selected track |
| 5      | Launch a clip at currently selected slot   |
| 6      | Arm currently selected track               |


Setup:

There are two parts of the puzzle of getting Pacer to properly talk with Ableton Live. You need a Pacer preset and Ableton Live script. 

Stage 1: Setting up Pacer

1. Download Pacer Preset file from the repository (The one with .syx extension)
2. Connect Pacer to your laptop and go to https://studiocode.dev/pacer-editor/#/patch
3. Ensure Pacer is connected and correct ports are chosen in the "MIDI input" and "MIDI output" dropdowns. (typically should be set to PACER MIDI1)
4. Click 'Load sysex file' and upload the Pacer Preset file.
5. Click 'Send to Pacer'. WARNING! This might overwrite your A1 slot. If you want to keep the preset stored there copy it to another slot first.

Stage 2: Setting up the control surface script

1. Download Nektar Pacer folder from the repository
2. Find your Ableton Live app in Applications folder. Right-click the app -> Show Package Contents. Navigate to Contents/App-Resources/MIDI Remote Scripts. Drop the Nektar Pacer folder into the MIDI Remote Scripts folder.
3. Start Ableton Live. Go to Preferences -> Link/MIDI tab. Under Control Surface dropdown you should now see Nektar Pacer option. Choose that. Set Input and Output to PACER (MIDI1). Below enable "Track" and "Remote" options for Nektar_Pacer Input (PACER (MIDI1)). Enable "Sync" and "Remote" for Nektar_Pacer Output (PACER(MIDI1)).

That's it! You should now be able to use the Pacer as discribed above. 

Please feel free to [drop me a DM](https://twitter.com/ivanibash) if you have any questions.
