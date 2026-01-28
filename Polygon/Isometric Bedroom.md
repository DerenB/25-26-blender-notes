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



# Create a Window

- Move the origin point to the plane where the window will be
  - Select the plane that will get the window
  - Select the face
  - `SHIFT + S` > Cursor to Selected
- Go Back into Object Mode
- Add Plane
  - Rotate on X 90 degrees
  - Adjust size and position
- Duplicate Plane
- Make one of the planes wider than the wall `E`
- Add the BoolTool extension if not already
- Add Hole
  - Rename large block plane
  - Add boolean modifier from BoolTool: `CTRL + -` (minus sign on numpad)
  - Move Boolean modifier to above bevel modifier
- Move First Window plane inset a bit into the wall

### Window Edge

- `CTRL + R` circle cut for bottom section of edge
- `P` separate it out
- Extrude it out
- Copy bevel modifier to it

### Window Frame

- Inset the main pane
- Separate the pane out
- Extrude the remaining frame to size
- Copy bevel to the frame

### Combine Parts into One Object

- Select the parts
  - Window Pane
  - Window Frame
  - Window Edge
- Select boolean invisible box last
- `CTRL + P` > Object



# Create the Bed

- `SHIFT + RMB` the origin point somewhere into the room
- Start with a plane
- Turn it into a box with extrude
- Create bed pillar with another plane
  - Mirror modifier the bed posts around the bed
  - Keep the bed/origin point the same so that the mirror works
- Once height is all set, apply the modifier

### Create Head Board

- select inner edges of head pillars
- Duplicate, `p` separate
- Go out and into edit mode with the new edges
- Select all > fill the faces
- Adjust the height of the board
- Subdivide the top edge
- Drag the outside verteces down (make the board into a point)
- `CTRL + SHIFT + B` to add a boolean and round the top
- Thicken plane with Extrude
- Duplicate > Separate > move to foot of bed
- Adjust foot of bed board height

### Mattress

- Duplicate and separate the top face of the bed frame
- Thicken with extrude
- Adjust width and length to fit the bed
- Loop Cuts
  - Add a loop cut parallel to the bed near the bottom
  - Add 2 loop cuts hamburger style around the mattress
    - Move these 2 to the head and foot of the bed, more space than the bottom one
  - Add 2 more loop cuts hotdog style
    - Also move to edges of bed
    - Can move by selecting the loop with `ALT` and move with `G`
- Add Subdivision modifier, 2 divisions
  - If bed too round, adjust where the loop cuts are

### Bevels

- Copy the same bevel modifier to the bed objects (not the mattress)
- Shade smooth

































