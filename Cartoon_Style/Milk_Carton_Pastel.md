# Pastel Cartoon Style Notes

# Transparency Material Shader

- Set up Render:
  - Set to Eevee
  - Color Management
    - Render > Color Management > View
    - Set to "Standard"
- Set up Material
  - All 3 into Mix Shader
    - Geometry Node (Backfaceing)
    - Transparent BSDF
    - Emission
  - Mix Shader into Material Output (Surface)
- Set Material Setting
  - Material > Settings > Surface > Render Method
  - Set to "Blended"



# Black Outline (Behind Object)

- Add 2nd material to object (plus icon)
- Enable Backface Culling
  - Material > Settings > Surface > Backface
  - (have to test if both Camera and Shadow is needed)
- Add Solidify Modifier
  - Normals > Flip: Enable
  - Materials > Material Offset: Set to 1 (or location of back color)




























































