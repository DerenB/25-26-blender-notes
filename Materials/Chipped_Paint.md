# LABEL GEOMETRY NODE

- Select Node, hit `F`
- Creates box with label at top



# CREATE NODE GROUP

- Select all nodes except the output node (Material Output)
- Join together: `CTRL + G`
- Hit `TAB` to toggle between node group and node view
- Assign input values
  - Drag points off the "group input" node into points in the material
  - Can change settings for input in the "group" tab on the right
  - Scale
    - Set type to "float"
    - Set default to 1
  - Drag as many values as you want



# Set up the Preview Sphere

- Add an icosphere
- Set sub divisions to 6
- Shade smooth
- Set Size to 0.2
- Apply scale `CTRL + A`



# Set up the Camera and lights

- Point camera at the sphere
- Set focal length to 80
- Set up 3 area lights



# HDRI

- Download HRDI
- Properties > World
- Set "color" to "environment texture"
- Open the HDRI .exr file
- Hide HDRI
  - Render > Film 
  - Turn on "Transparent"



# Color Management

- Render > Color Management
- Set Dispaly to sRGB
- Set View to AgX
- Set Look to Very High Contrast


