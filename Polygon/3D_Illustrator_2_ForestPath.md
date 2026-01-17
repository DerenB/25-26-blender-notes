
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



