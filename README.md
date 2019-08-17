# Outdoor solar harvester

![assembly_165x165_MCP73871_BLM.gif](https://github.com/panovvv/solar-harvester/raw/master/media/assembly_165x165_MCP73871_BLM.gif?raw=true)

## Supported hardware
* Solar charger boards: CN3065, CN3791, MCP73871, TP4056 both shortened and full-size boards.

![charger_boards.jpg](https://github.com/panovvv/solar-harvester/raw/master/media/charger_boards.jpg)

* Solar panel sizes: 90x70mm and any arbitrary size upwards of that, limited only by printing volume and your imagination. Pre-made sizes (you'll find ready STL files for all those sizes in stl/ folder):

```
● 110x110
● 112x84
● 115x85
● 125x110
● 130x110
● 135x135
● 136x110
● 138x82
● 145x145
● 165x130
● 165x135
● 165x165
● 200x130
● 213x92
● 220x170
```

Down to 80x65mm (which is the size of the central opening where electronics is housed) is doable, but there'll be some extra space around the panel. 

For solar panels smaller than 80x65mm and any sizes not readily available under stl/ folder, you'll have to customize the part under enclosure/front/solar_panel_frame.ipt

* Battery: any 18650 lithium cell, with 2 types of holders: CGS and BLM:

![battery_holders.jpg](https://github.com/panovvv/solar-harvester/raw/master/media/battery_holders.jpg)

## BOM and detailed instructions

Refer to this blog post: [Homemade solar harvester to power your outdoor projects](https://www.shortn0tes.com/2019/07/solar-harvester.html).

Version 2 specific info and updated assembly instructions are here: [Outdoor solar harvester v. 2.0](https://www.shortn0tes.com/2019/09/solar-harvester-v2.html).

I recommend at least skimming through both posts, because essential details/tips and tricks are all over both of them.

## Description of contents

Modeled with Autodesk Inventor 2018

* enclosure/ - Inventor models of enclosure. Those are exported as STLs to stl/ folder.
  * front/ - frontal part of enclosure. Solar panel is glued to it, and the waterproof connector goes in here too. There's only one file, solar_panel_frame.ipt, and it's suitable for all panel sizes.
  * back/ - back lid. You attach the battery and the charging board to it.
  * washer/ - template for silicone/rubber washer that goes 
  between front and back parts of harvester - this is one of the measures we undertake to make it watertight.

* step/ - same models as in enclosure/ directory, STEP file format. 

* stl/ - folder with 3D printed parts. This is what you're here for.
  * front/ - pre-made frontal parts for common solar panel sizes, plus one generic part for 100x100mm panel.
  * back/ - permutations for all battery holder + charger board combinations. Also gizmos to hold some of the chargers in place.

* solar_harvester_*.iam and  - full assembly of finished device.

* solar_harvester_*.ipn - presentation file with exploded view.
When rendered in reverse, results in video with assembly instructions.

* parts/ - Inventor models of constituent electronics (i.e. everything not hand-crafted).

* media/ - rendered stills and videos: exploded views, turntable animations, etc.