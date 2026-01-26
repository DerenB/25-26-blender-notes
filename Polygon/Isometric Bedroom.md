# Isometric Bedroom

- Add floor plane
- Separate and extrude the back 2 walls



# Setup Camera

- Set to Orthographic
- Set resolution (3:4 in demo)
- Adjust Orthographic scale for zoom in/out



# Walls

- Add thickness
  - Edit mode
  - `A` > `ALT + E` > Extrude Faces along normals
  - Use `S` to keep it parallel
- Make sure faces are oriented correctly



# Floor

- Scale to slightly larger than the walls
- Circle cut into boards (6-7)
- Hit `V` > `RMB` to separate them
- Add vertices
  - Select the end edges of the panks
  - `RMB` > Subdivide
  - Going into vertex select mode should show the new vertices in the middle
- Round the Boards
  - Select all of the middle vertices
  - Move them outwards in Y direction, so the end is a zig zag shape
  - `CTRL + Shift + B` to bevel them, 4-5 times, makes the ends of the boards round
- Stagger the board
  - Select 3-4 boards to move
  - Deselect everything except the edges of the boards `CTRL + LMB Drag`
  - Move back
- Extrude Boards Down
- Fix face orientation `SHIFT + N`



# Bottom Floating Platform

- Add a plane
- Widen it to width
- Extrude down
- Bevel Corners
  - Can select the 4 edges with `CTRL + Alt LMB`
- Double check face orientation



# Top Beam Platform

- Select top of the walls
- Duplicate `shift + D` and separate `p`
- Select new duplicate in edit mode
- Extrude Upwards
- Scale outwards `ALT + S` and do it evenly with second `S` click



# Bevel Floor Boards

- Add bevel modifier to the floor boards
- Settings (whatever looks right):
  - Amount: 0.015
  - Segments: 3
  - Geometry > Miter Outer: Arc
  - Shading > Harden Normals: Checked
- Apply the modifier to every object (walls, ceiling, platform)
  - Select every object, select floorboards last
  - Can click "copy to selected" in the modifier menu



# Cut a Window

- Move the origin point to the plane
  - Select the plane that will get the window
  - Select the face
  - `SHIFT + S` > Cursor to Selected































