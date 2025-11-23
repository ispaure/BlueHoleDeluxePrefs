Here is the list of Pie Menus for Blue Hole.

> [!NOTE] Dependencies
> **Note that the Deluxe edition of Blue Hole is required for any Pie Menu shown here.**
> Added dependencies are noted (whenever applicable). The menu would still popup but some option(s) may be missing, with shown warnings.


# 🧊 Object Mode
---
These menus are unique to **Object Mode**.
## 🍰 Tool
Keymap: `Shift + RMB Drag`
Additional dependencies: [HardOPS](https://superhivemarket.com/products/hard-ops--boxcutter-ultimate-bundle).
```mermaid
graph TD

    %% Nodes
    NW["Weighted Normal"]
    W["Lattice"]
    SW["Subdivide"]

    N["*Modifier Options...*"]
    C["**TOOL (Object) PIE**"]
    S["Modifier Toggle"]

    NE["Twist Array"]
    E["Array"]
    SE["Radial Array"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Modifier Options** → Link/Transfer Data, Apply Modifiers_

## 🍰 Action
Keymap: `Ctrl + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Apply Object Transform"]
    W["Clear Location"]
    SW["Clear Parent"]

    N["*Select...*"]
    C["**ACTION (Object) PIE**"]
    S["*More...*"]

    NE["Quick Pivot Setup"]
    E["Join"]
    SE["Make Parent"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Select** → Select Grouped, Select Parent, Invert, Select Children  
**More** → Convert to Mesh, Apply Modifiers, Make Instances Real, Clean, Convert to Curve_



# 🛠️ Edit Mesh Mode
---
These menus are unique to **Mesh Edit Mode**, which corresponds to **Vertex**, **Edge** and **Face** selection.
## 🍰 Tool
Keymap: `Shift + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Knife Topology Tool"]
    W["Bevel"]
    SW["Bridge Edge Loops"]

    N["Loop Cut and Slide"]
    C["**TOOL (Mesh) PIE**"]
    S["Inset Faces"]

    NE["Extrude and Move on Individual Normals"]
    E["Extrude and Move on Normals"]
    SE["Shrink/Fatten"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```

## 🍰 Action (Vertex)
Context: **Vertex Edit Mode**
Keymap: `Ctrl + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Straighten"]
    W["Merge Last"]
    SW["Merge by Distance"]

    N["*Select...*"]
    C["**ACTION (Vertex) PIE**"]
    S["*More...*"]

    NE["Quick Pivot Setup"]
    E["Merge to Center"]
    SE["Connect Path"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Select →**_ _Random, Invert, Loose Geometry_  
_**More →**_ _To Sphere, Symmetrize, Quick Flatten, Vertex to Circle, Quick Lattice_

## 🍰 Action (Edge)
Context: **Edge Edit Mode**
Keymap: `Ctrl + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Grid Fill"]
    W["Edge Split"]
    SW["Clear Sharp"]

    N["*Select...*"]
    C["**ACTION (Edge) PIE**"]
    S["*More...*"]

    NE["Quick Pivot Setup"]
    E["Edge Crease"]
    SE["Mark Sharp"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Select →**_ _Smart Loop, Sharp Edges, Invert, Smart Ring, Loop Inner-Region_  
_**More →**_ _Subdivide Edge-Ring, Rotate Selected Edge (Right), Quick Pipe, Rotate Selected Edge (Left), Mesh Angle, Collapse_

## 🍰 Action (Face)
Context: **Face Edit Mode**
Keymap: `Ctrl + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Quick Lattice"]
    W["Split"]
    SW["Merge by Distance"]

    N["*Select...*"]
    C["**ACTION (Face) PIE**"]
    S["*More...*"]

    NE["Quick Pivot Setup"]
    E["Separate"]
    SE["Separate Loose Parts"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Select →**_ _Boundary Loop, Linked Flat Faces, Invert, Loose Geometry, Random_  
_**More →**_ _Poke Face, Recalculate Normals Inside, Recalculate Normals Outside, Subdivide, Tris to Quads, Flip, Triangulate Faces, Un-Subdivide_

## 🍰 Action UV Special (Vertex, Edge, Face)
*This menu has **UV-related** options. It is available from all three **Vertex**, **Edge** and **Face** modes.*
Keymap: `Ctrl + Alt + Shift + RMB Drag`
Additional dependencies: [ZenUV](https://superhivemarket.com/products/zen-uv), [DreamUV](https://github.com/leukbaars/DreamUV)
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Fix Trim Loop"]
    W["Clear Seam"]
    SW["Auto Unwrap"]

    N["Hotspot"]
    C["**ACTION UV SPECIAL**"]
    S["Zen Unwrap"]

    NE["Fit to Trim"]
    E["Mark Seam"]
    SE["Mark by Angle"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```



# 🍑 Curves
---
These menus are unique to the **Curve Edit Mode**.
## 🍰 Tool
Keymap: `Shift + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Tilt"]
    W["Make Segment"]
    SW["Decimate Curve"]

    N[" "]
    C["**TOOL (Curve) PIE**"]
    S["Smooth"]

    NE["Scale"]
    E["Extrude Curve and Move"]
    SE["Subdivide"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```

## 🍰 Action
Keymap: `Ctrl + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Recalculate Handles"]
    W["Split"]
    SW["Switch Direction"]

    N["Smooth Curve radius"]
    C["**ACTION (Curve) PIE**"]
    S["Dissolve Vertices"]

    NE["Set Handle Linear"]
    E["Separate"]
    SE["Toggle Cyclic"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```



# 🖌️ Sculpt
---
These menus are unique to the **Sculpting** mode. They include all the brushes that come by default with Blender.
## 🍰 General
Keymap: `Shift + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW[" "]
    W["*Flatten/Pinch...*"]
    SW["*Misc...*"]

    N["*Clay/Blob...*"]
    C["**GENERAL**"]
    S["*Grab...*"]

    NE["*Draw...*"]
    E[" "]
    SE[" "]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Clay/Blob →**_ _Clay, Fill/Deepen, Clay Thumb, Clay Strips, Blob, Layer  
**Draw →** Draw, Draw Sharp_  
_**Grab →**_ _Grab Silhouette, Elastic Snake Hook, Snake Hook, Nudge, Thumb, Grab 2D, Elastic Grab, Grab  
**Misc →**_ _Density, Face Set Paint, Relax Slide, Smear Multires Displacement, Twist, Mask, Relax Pinch, Erase Multires Displacement  
**Flatten/Pinch →**_ _Boundary, Scrape/Fill, Scrape Multiplane, Trim, Smooth, Plateau, Flatten/Contrast, Pinch/Magnify_

## 🍰 Paint
Keymap: `Ctrl + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Sharpen"]
    W["Paint Soft"]
    SW["Paint Soft Pressure"]

    N["Paint Square"]
    C["**PAINT**"]
    S["*Blend/Blur...*"]

    NE[" "]
    E["Paint Hard"]
    SE["Paint Hard Pressure"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Blend/Blur** **→**_ _Paint Blend, Blend Square, Blend Hard, Blend Soft, Smear, Airbrush_

## 🍰 Simulation
Keymap: `Ctrl+ Alt + Shift + RMB Drag`
Additional dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Grab Planar Cloth"]
    W["*Expand/Contract...*"]
    SW["*Bend/Stretch/Twist...*"]

    N["Grab Cloth"]
    C["**SIMULATION**"]
    S["Pinch Point Cloth"]

    NE["Grab Random Cloth"]
    E["Grab Cloth"]
    SE["Pinch Folds Cloth"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Bend/Stretch/Twist →**_ _Twist Boundary Cloth, Bend/Twist Cloth, Stretch/Move Cloth, Bend Boundary Cloth  
**Expand/Contract →**_ _Inflate Cloth, Push Cloth, Expand/Contract Cloth_



# 🗾 UV Editor
---
These menus are unique to the **UV Editor** 2D View.
## 🍰 Tool
Keymap: `Shift + RMB Drag`
Additional dependencies: [ZenUV](https://superhivemarket.com/products/zen-uv)
```mermaid
graph TD

    %% Nodes
    NW["Quick Mirror"]
    W["Smart UV Project"]
    SW["Auto Unwrap"]

    N["Quick Rotate"]
    C["**TOOL (UV) PIE**"]
    S["Zen Unwrap"]

    NE["Quick Fit"]
    E["Relax"]
    SE["Relax Along U"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```

## 🍰 Action
Keymap: `Ctrl + RMB Drag`
Dependencies: [ZenUV](https://superhivemarket.com/products/zen-uv)
```mermaid
graph TD

    %% Nodes
    NW["Get Texture Density"]
    W["Quadrify"]
    SW["Split Island"]

    N["*Select...*"]
    C["**ACTION (UV) PIE**"]
    S["Merge UV Verts"]

    NE["Set Texture Density"]
    E["World Orient"]
    SE["Stitch"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
_**Select →**_ _Select Interseam Loop, Select Seams Edges, Select Flipped Islands, Select Overlapped Islands, Select Similar Islands, Select Split Edges, Select Stretched Faces, Select UV Borders_

## 🍰 Action (Special)
Keymap: `Ctrl + Alt + Shift + RMB Drag`
Dependencies: [ZenUV](https://superhivemarket.com/products/zen-uv)
```mermaid
graph TD

    %% Nodes
    NW["Fix Trim Loop"]
    W["Quadrify"]
    SW["Pack Islands"]

    N["Select Trim Tool"]
    C["**ACTION (Special) PIE**"]
    S["Zen Unwrap"]

    NE["Fit to Trim"]
    E["World Orient"]
    SE["Relax Along U"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```

## 🍰 Cursor
Keymap: `Ctrl + Shift + RMB Drag`
Dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["to Selected"]
    W["*UV TOOLKIT Option to Remove*"]
    SW["to Pixel"]

    N[" "]
    C["**CURSOR**"]
    S[" "]

    NE["to Cursor (Offset)"]
    E["to Cursor"]
    SE["to Pixel"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```



# 💾 File Management
---
## 🍰 Directories
Keymap: `F3`
Dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["Add ASSET HIERARCHY"]
    W["Open WORKSPACE ROOT Folder"]
    SW["Open USER RESOURCE PATH"]

    N["Open ROOT Folder"]
    C["**DIRECTORIES PIE**"]
    S["Open FINAL Folder"]

    NE["Open RESOURCES Folder"]
    E["Open SPEEDTREE MSH Folder"]
    SE["Open REFERENCES Folder"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```

## 🍰 Import / Export
Context: This menu functions in **Object Mode only**.
Keymap: `Ctrl + Alt + Shift + RMB Click`
Dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW["*Open Directories...*"]
    W["*Extra...*"]
    SW[" "]

    N["*Source Control (Perforce)...*"]
    C["**IMPORT/EXPORT PIE**"]
    S["*Send...*"]

    NE["Add Asset Hierarchy"]
    E["*Export...*"]
    SE[" "]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```



# 🙋‍♂️ Help
---
Keymap: `F1`
Dependencies: N/A
```mermaid
graph TD

    %% Nodes
    NW[" "]
    W[" "]
    SW["*Themes...*"]

    N[" "]
    C["**HELP PIE**"]
    S["❤️Submit Feedback"]

    NE["Online Guide"]
    E["Keymaps List"]
    SE["Pie Menus List"]

    %% Fake links for positioning
    NW --- W --- SW
    N --- C --- S
    NE --- E --- SE

    %% Hide all connectors AND arrowheads
    linkStyle default stroke:transparent,stroke-width:0;
```
