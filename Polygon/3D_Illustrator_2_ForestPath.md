
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
  - 

