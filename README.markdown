SVG2VoxMap 
================================

About
---

A Basic droplet app written in AppleScript, which takes a source SVG file, and outputs a Castle Vox Map file (.voxb)




Download & Installation
---

Run the unit tests with a local server that supports PHP. No database is required. Pre-configured php local servers are available for Windows and Mac. Here are some options:

[Download here](https://github.com/downloads/lukejcam/svg2VoxMap/SVG2VoxMap.zip)

To Install, simply unzip and drag the app to applications folder. Drag a shortcut to your dock.


Usage
---

Drag and drop an svg source file onto the dock icon, the vox map file will be created in the same directory
as the source file.

Things to note
---


- Because of the way Castle Vox maps work, only the polygon tags will be used. Paths (Basically anything that uses a bezier curves is a path) be ignored.
- Layers and groups can be used as, the script will recursively search the entire file for polygon tags, ignoring the group and layer tags.
- The source SVG does not have to be flipped vertically. The source coordinates are reversed and inversed accordingly.