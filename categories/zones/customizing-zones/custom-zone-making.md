---
description: This guide covers custom zone making and the tooling available
---

# Custom Zone Making

Currently, one of the most developed ways to do custom zones is the OpenZone tool. There are many tools available to export original EQ zones to various formats, but making zones is an area not as heavily developed. 

### Making Zone Options

Openzone supports the following flows to import and generate zones:

| Flow | Ext | Pros | Cons |
| :--- | :--- | :--- | :--- |
| OpenZone \(.scn\) | .scn | All features available | Very clunky, camera movement horrible, have to type in coordinates |
| 3d Studio Max | .3ds | Native modeling controls | Unverified if works with latest version, might have poly limits? |
| Quake 3 | .bsp | Ongoing updates, easy UI, free | TBD |
| Dungeon Builder | .3ds | TBD | TBD |

### Quake 3 Map Import

#### 

1. Download [https://github.com/Garux/netradiant-custom](https://github.com/Garux/netradiant-custom) netradiant custom. 
2. Extract netradiant to any path you prefer
3. Download openzone, I've had the best luck with 8.3 as of oct 2021
4. Open radiant.exe
5. Inside your openzone dir, there should be a library directory, create this following style of paths: &lt;openzone dir&gt;/library/textures/quake3
6. Create an empty path and call it baseq3, for example: [https://github.com/demoncia/client/tree/main/radiant/baseq3](https://github.com/demoncia/client/tree/main/radiant/baseq3)
7. Create a maps folder
8. Create a shaders folder
9. Create 

