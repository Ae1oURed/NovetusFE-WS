# NovetusFE-WS
NovetusFE Workshop Store

# Rules
Since Novetus is quite a small community I doubt that a huge number of commits is going to happen, so we should be fine for now. However, I still have rules, No malware, no attempts at griefing, no nsfw or lewd addon icons. If you break one of these rules I will not add your project or mod to the workshop and if you get a project added but break rules after then I will remove your project from the workshop and never add it back.

# Example
store.json
```
{
	"shortname":"CharCommands",
	"longname":"Character Commands",
	"description":"Robloxian 2.0 Addon for Novetus",
	"creator":"Lachrymogenic",
	"tags":["addons"],
	"url":"https://github.com/Lachrymogenic/CharacterCommands/archive/refs/heads/main.zip",
	"iconurl":"https://raw.githubusercontent.com/Lachrymogenic/CharacterCommands/main/charcustom.png",
	"indexlocation":"CharacterCommands-main/index.txt",
	"leaveout":true,
},
```    
index.txt
```
CharacterCommands-main/addons/CharacterCommands.lua
```

# How to add your Project / Mod to the Workshop?
![](https://raw.githubusercontent.com/Lachrymogenic/NovetusFE-WS/main/example.gif)
First, create an index.txt file for your mod / project, this file will contain a list of every file you wish to be extracted from within a zip file. For an example of how to create an index.txt, see my example project here, https://github.com/Lachrymogenic/CharacterCommands The format is usually "modname-main/(addons / models / sounds / whatever)/(if you have extra folders: folder-name / )your-file Make a commit to store.json and make sure you format it correctly, do not forget commas etc.

# Legend
## shortname
A shortname is a short name for the Compact theme of NovetusFE, string.
## longname
A longname is a long name for an Extended theme of NovetusFE, string.
## description
A description for your mod / project, string.
## creator
The creator of the mod / project, string.
## tags
Search tags to make finding your mod / project easier, (e.g "addons" or "place" or "models" or "themes"), strings in array.
## url
The URL which NovetusFE will use to download your mod / project, string.
## iconurl
The URL which NovetusFE will use to download your mod / project's Icon. (128x128), string.
## indexlocation
Location of index.txt inside of the zipfile, string.
## leaveout
If you are using Github, set this to true, as leave out will take the first folder in a zip file and treat it as if it were the root folder, if everything is correctly in the root of the zip file, and the structure is ./addons and not ./Project-main/addons, then you can set this to false, bool.
