
# Increase Vertices Size

- Edit > Preferences > Themes > 3D Viewport
- Vertex Size 

# Create Dead Tree

- Get down to 1 vertex
  - Add a plane
  - Select all 4 vertices
  - Merge `M` at center
- Create height
  - extrude single vertex upwards `E`
- Create branches
  - Add loop cuts `CTRL + R`
  - Group the loops together with `S`
  - Create as many vertices in a group as you want number of branches
- Create Branches
  - Extrude loop cut vertices outwards to create branches
- Rotate branches to how you want
- Skin Modifier
  - Add Skin Modifier for thickness
- Decimate Modifier
  - Use a Decimate modifier to reduce the number of faces (low poly)



# Create Rock

- Add Cube
- Add subdivide 1, Apply
- Change shape
  - Adjust height
  - Bisect Tool
    - Under the Knife Tool
    - Hold `LMB` to select the bisect



### Skin Modifier

- Add skin modifier to thicken vertices
- adjust thickness
  - in edit mode
  - show side panel `n`
  - Adjust Mean Radius X/Y
  - Can adjust with `CTRL+A`



# Terrain

- Create Plane
- Sub divide 4 times
- Extrude up
- Hide bottom vertices
- Create River
  - Select right 4 rows of vertices
  - Drag downwards 
- Triangulate Faces
  - Select all
  - Face > Triangulate
- Add Bumps to terrain
- Can hide vertices so they aren't affected by editing
  - Hide the bottom of the platform so it stays flat
  - Hide the edge perimeter so it stays straight
- Adjust river x-axis to create uneven edge
- Add random adjustments
  - Turn on proportional editing `O`
  - Set to Random
- Create road
  - unhide everything and turn off proportional editing
  - Select 4 columns in the middle
  - Scale `S` in the `Z` axis
  - Drag to 0 or hit `0`
  - This will make them uniformly flat
  - Lower into the ground a bit
- Recalculate Normals
  - Done just to be safe
  - Edit Mode
  - Select all `A`
  - Recalculate `SHIFT + N`



# Create Water

- Add a plane
- Position it just inside the edge of the terrain and just below the river bed
- Add 3 loop cuts (4 sections)
- Subdivide a few times
- Extrude the water up
- Recalculate Normals
  - Done just to be safe
  - Edit Mode
  - Select all `A`
  - Recalculate `SHIFT + N`



### Vertex Group

- Select top face vertices
- Properties > Data
  - Lets you explore the data that is within the object
- Vertex Groups > "+" icon
  - Assign the vertices to it
  - Can test it by deselecting the vertices, then clicking "select", should select all of them
  - Name the group
- Object Mode Displace
  - Object Mode
  - Add modifier "Displace"
  - Assign the previously created vertex group
  - Set Direction to "Z"
  - Create Texture
    - Within modifier > New
    - Rename the Texture
  - Edit Texture
    - In Properties > Texture
    - Set Type to "Clouds"
    - Set Size to 1
  - Adjust bump height
    - Back in Displace Modifier
    - Set the Strength value
    - Set to 0.460
  - Triangulate Surface
    - Select top surface group with the vertex group
    - `CTRL + T` to triangulate



# Modify Road

- Select the road faces
- Duplicate and separate the road
- Add waves/grooves to the side of the road
- Extrude it upwards
- Recalculate Normals just in case



### Create Lines in Road

- Add a plane
- Shape it into a line in edit mode
- Duplicate it with modifier
  - Use "Array" modifier
  - Set Count
  - Set relative Offset Y (to copy over the y axis)
- Solidify
  - Add Solidify modifier



# Add Assets

- Snapping Objects
  - Turn on Sanp at top
  - Set to Face Project
  - Hold `CTRL` to disable snapping while holding an object
- Track Ball Rotate
  - Hit `R` twice
- Add Rocks how you want
- Add trees how you want
- Add dead trees how you want



# Materials

- Water Material
  - Set Transmission to 1
  - Set Roughness to 0.2
  - Set IQR to 1.333



# Create Isometric Camera

- Return cursor to world origin
  - `SHIFT + S` > Cursor to World Origin
- Add a Camera
- Set Camera Rotation
  - X-Axis: 54.7
  - Z-Axis: 45
- Change Camera to Orthographic
  - Done in the camera properties
- Camera distance
  - Moving the camera does nothing in orthographic
  - Have to set the "Orthographic Scale", example is 14
- Ratio
  - 4-to-3 is his most common isometric camera angle
  - The rotation 54.7-to-45 is the same 4-3 ratio
  - More on top angle is 1-to-1
  - More angled, low to ground angle, is more like 2-to-1



# Render & Lights

- Limit Render Preview
  - `CTRL + B`
  - Draw around the camera bounds
- Render Settings
  - Turn on Denoise
  - Set to OptiX
- Add a sun
- Add an area light



# Texture Painting Puddles

- Unwrap (UV Editor)
  - Need to unwrap a 3D object into a 2D one to texture Paint it
  - Select All > Smart Unwrap with `U` > Smart Unwrap > Use default settings
- Set up
  - Set left screen to Image Editor > Set to "Paint" mode
    - Can split left screen to add "shader editor"
  - Right Screen: Select object > Object Mode into Texture Mode
- Create Texture
  - In Texture Mode > Top > Texture Slot 
  - Should be "no textures", click "+" to create one
  - Use "Roughness" for the painting
  - Set to 2k textures 2048x2048
  - Set color, 0 for rough 1 for smooth
  - Set Value to 0.7
- Painting
  - Cycles does not automatically refresh texture painting
  - Just use material preview mode
- Set Brush Falloff / Blue
  - Properties > Tool > Falloff
  - Can select a default curve shape, like round preset
- SAVE THE TEXTURE
  - texture image is not automatically saved with `CTRL + S`
  - Embed image
    - Image > Pack
    - This packs the image into the blender file
    - Still need to manually save the file everytime
  - View Embedded files
    - Scene Window
    - Display Mode > Blender File
      - Open Images tab
    - Original screen is View Layer



# Rendering

- Cycles
- GPU Compute
- Samples 4,096
- Denoise
  - OptiX
  - Albedo and Normal
- Color Management (this example)
  - Filmic
  - Medium High Contrast


