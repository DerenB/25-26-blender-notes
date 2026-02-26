# Cloth

# Hanging Towel Tutorial

- Add Plane
- Make it an rectangle that is 2x wide
  - Then you can `CTRL R` circle cut and have 2 even squares
- Subdivide ~35 times (enter in the menu)

### UV Unwrap

- Unwrap the object now before deforming if you are going to
- Click "UV Editing" at top
- `U` > Unwrap Angle Based

### Add Cloth Physics

- Add Cloth Modifier OR click "cloth" in physics tab

### Create Pin Group

- Select vertices that should be pinned and not move
- Properties > Data
- Create a new vertex group with "+" icon
- Click "Assign" to assign selected vertices to the group
- Add pin group to physics
  - Back in Physics tab
  - "Shape" > Pin Group
  - Select the created Pin Group

### Self Collisions

- Physics > Collisions > Self Collisions
- Set Distance
  - If too high, cloth will bunch up
  - Tutorial set to 0.005

### Quality Steps

- Higher number, higher quality but more demanding
- Tutorial set to 10

### Vertex Mass

- Physical Properties > Vertex Mass
- Sets the weight of the towel
- Tutorial set to 0.5

### Bending

- Stiffness > Bending
- Higher number, less bending
- Tutorial set to 10

### Solidify

- Add cloth modifier first, then solidify
- DON'T add before cloth
  - It will try to simulate both sides of the cloth

### Subdivision

- Add 3rd, after cloth and solidify
- Adds smoothness
- DON'T add before the cloth
  - Will add too many vertices to simulate





# Setup

- Turn on "Collision" for any object the cloth will touch
  - Properties > Physics > Collision



# Subdivisions

- Need to subdivide the plane for the cloth to function
- Subdivide manually
  - Can right click and subdivide, but it is destructive
- Modifier
  - Can add a subdivide modifier, but it is also destructive



# Geometry Nodes

- 












