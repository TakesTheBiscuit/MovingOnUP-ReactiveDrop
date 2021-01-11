# MovingOnUP-ReactiveDrop - how to build

## How to compile .vpk needed

Now that you have your files laid out in a folder, you need to pack them into a VPK, or Valve PacK file.

In Steam, right click on Alien Swarm: Reactive Drop and select Properties. On the Local Files tab, click Browse Local Files.... Double click on the bin folder and find vpk.exe. Drag your add-on folder onto vpk.exe and a VPK file with the same name as your folder should appear.

Important things to note:

Alien Swarm: Reactive Drop uses VPK version 1, which only allows one dot per filename. This is especially important for models: make sure you only have a .dx90.vtx so it doesn't get overridden by one of the other vtx files.

VPK files can be opened by freely available tools such as GCFScape. Any file you put into the VPK will be accessible to anyone who downloads your add-on.

All add-ons share the same filename space, along with the game. This means that if your add-on includes a different file with the same name as a file in another add-on, one of the two add-ons will likely break. It is important that any file you create specifically for your add-on has a unique name. This can be as simple as putting the name of your campaign in the name of a texture file, and so on.

### Source of info:
https://steamcommunity.com/sharedfiles/filedetails/?id=874942353


## Deviations

Had to copy vpk.exe to `{drive}:\Steam\steamapps\common\Alien Swarm Reactive Drop\bin` as it requires some .dll files from that location.

## Running vpk.exe
- Open powershell -> admin
- Run: `.\vpk MovingOnUP-ReactiveDrop -v`
- Find movingonup.vpk file

## Publishing
Use in-game workshop -> upload tool