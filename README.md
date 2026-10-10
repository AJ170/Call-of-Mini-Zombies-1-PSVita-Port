## IMPORTANT
Create a folder called `comZombiesOffline` in `ux0:data` should look like
```
ux0:
  └── /data/
        └── /comZombiesOffline
```

# Call-of-Mini-Zombies-1-PSVita-Port
Credit to Triniti for making the game.
Credit to Overmet15 for decompiling the game.

<img width="960" height="544" alt="2026-10-10-203259" src="https://github.com/user-attachments/assets/72aa39f5-ffa2-4311-862e-539648bcd47c" />

## Controls
```
square - Shoot
triangle - Change Weapons
start - Pause
Left Stick - Move Character
Right Stick - Move Camera
R - Shoot
DPad Left - Consume Item 1
DPad Right - Consume Item 2 
```

## Installation

No VPK is provided directly. Release contains an xdelta patch that must be
applied to your own copy of the original game.
You need version 4.4.2 of Call of Mini Zombies 1 .apk file for android (MUST BE ORIGINAL GAME FILES) and RENAME the .apk to `COMZ.apk`

1. Install `CoMZombies_v1.01-stub.vpk` on your Vita with VitaShell or VitaDB
2. Download [xdelta3](https://github.com/jmacd/xdelta) ([Windows builds here](https://github.com/jmacd/xdelta-gpl/releases)) and put `xdelta3.exe`, the renamed .apk file and `COMZData.xdelta` in the same folder
```
Newly Created Folder
└── /COMZ.apk
└── /COMZData.xdelta
└── /xdelta3.exe
```
3. Open a command prompt in that folder and run:     

`./xdelta3 -d -B 1073741824 -s COMZ.apk COMZData.xdelta COMZData.zip`

4. Extract `COMZData.zip` and copy the "Media" folder into `ux0:app/COMZ42069/`
and merge with the existing files
5. Launch Call of Mini Zombies
