# Hard Surface Notes

- Random notes on Hard Surface topics

### Table of Contents

- [Hard Surface Notes](#hard-surface-notes)
    - [Table of Contents](#table-of-contents)
- [Bevel Modifier](#bevel-modifier)
- [Boolean Cut](#boolean-cut)
- [Mirror Boolean](#mirror-boolean)
- [Scale Evenly](#scale-evenly)
- [Shade Smooth Fix](#shade-smooth-fix)
- [Slice](#slice)
- [Union Objects](#union-objects)



# Bevel Modifier

- Set Number of segments
- Set Amount to low amount for small bevel
- Fix hard surface shading issues
  - Turn on Shading > Harden Normals
- Fix Corner Triangles
  - Some corners have weird triangle geometry
  - Set Geometry > Miter Outer > Arc



# Boolean Cut

- Use the addon "Bool Tool"
- Add the cutting object
- Select cutting object first
- `SHIFT` select object to be cut
- `CTRL + SHIFT + B` > Brush Boolean > Difference
- Make sure cut modifiers are above the bevel modifier



# Mirror Boolean

- Add mirror modifier
- Adjust the origin point to adjust it cutting
- Turn on Bisect



# Scale Evenly

- In edit mode: `ALT + S`



# Shade Smooth Fix

- Using "Shade Smooth" causes visual issues
  - Caused by shading trying to go over angled surfaces
- Use "Shade Auto Smooth"
- It adds a modifier "Smooth by Angle"
- Any surface transition that is greater that the input angle (30 default), will be shaded separately 



# Slice

- Select minor object first, then major
- `CTRL + SHIFT + B` (Bool Tool)
- Brush Boolean > Slice
- Makes a line slice into the object along the edges of the minor object
- Make sure cut modifiers are above the bevel modifier



# Union Objects

- Select minor object first, then major
- `CTRL + SHIFT + B` (Bool Tool)
- Brush Boolean > Union
- Make sure cut modifiers are above the bevel modifier











