# Hard Surface Panels

# Plane Example

- Add enough vertices/edges 
- Mark Sharp
  - Select as many edges as needed
  - `CTRL + E` > Mark Sharp
- EdgeSplit
  - Add the "EdgeSplit" modifier
  - turn off "Edge Angle"
- Solidify
  - Add Solidify modifier
  - Set thickness
  - Turn on "Fill"
  - Turn on "Only Rim"
- Bevel   
  - Add Bevel modifier
  - Set Amount (demo did 0.009)
  - Set Segments (demo did 3)
- Use modifiers in that order
  - Edgesplit
  - Solidify
  - Bevel
- Not Working
  - If it is not working, check for overlapping vertices
  - Merge with `M` by Distance



# Circle Shape

- Select the faces for the size of the cirle
- `RMB` > LoopTools > Circle
- Select the edges of the circle > `CTRL + ` > Mark Sharp



# Rounded Corners

- How to make your panels have soft corners instead of sharp 90 degree ones
- Add a subdivision modifier 2nd
- Order:
  - EdgeSplit
  - Subdivision
  - Solidify
  - Bevel



# Mix of Sharp and Soft Corners

- Edit Mode
- Select vertex at the corner you want to adjust
- Attribute Panel `N`
- Set the Vertex Data > Vertex Crease
  - 1 for Sharp 90 degree
  - 0 for soft rounded



# Separate Sections

- Go into edit mode
- Select every face of the panel
- Separate by Selection `P`
- Back into object mode and back into edit mode with only the new section
- Move up or down with `ALT + S`
- Increase/Decrease solidify modifier as needed

