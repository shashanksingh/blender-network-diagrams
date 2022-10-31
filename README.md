# blender-network-diagrams
Creating a Blender script to render Stylized Network [diagrams](https://github.com/shashanksingh/blender-network-diagrams/blob/master/Screenshot%202022-10-31%20at%2000.06.50.png)


Plan
1. get isometric setup done https://www.youtube.com/watch?v=yCHT23A6aJA 
2. then use diagram tool https://diagrams.mingrammer.com/ to convert it into blender script like

goal bare minimum look like https://www.cloudcraft.co/

import bpy
import random


#bpy.ops.camera.preset_add(name='ortho')
bpy.ops.mesh.primitive_plane_add(size=100,align='WORLD',location=(0,0,-1),enter_editmode=False)
bpy.ops.mesh.primitive_cube_add(size=2,align='WORLD',location=(0,0,0),enter_editmode=False)
bpy.ops.mesh.primitive_cube_add(size=2,align='WORLD',location=(0,3,0),enter_editmode=False)

and render it headless
