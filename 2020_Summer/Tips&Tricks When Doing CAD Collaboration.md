# Tips&Tricks When Doing CAD Collaboration

[TOC]

## Etiquette

1. Fully define the position of each part in assembly, unless visualization of motion needed for certain parts
2. Use part library/toolbox if available
3. Don’t release linked parts

## Sketches

1. Fully define sketches. All BLACK, no BLUE. DO NOT use “Fully Define Sketch” button
   Use equations, relations, and general variables
2. Use relation definitions (for example, “=”), or define variables
3. Combine Common Dimensions
4. Dimension rectangles from the edges, not the corner(解释)
5. Make separate features in separate sketch unless it’s master sketch from top-down
6. Use symmetrical relations
7. Put origin at a mounting location (or center point)
8. Use construction lines to help define sketch (减少trim)
9. 3D Sketch - 2D first then having 3D sketch come off of that

## Parts

1. Use symmetry whenever possible
2. Use configuration when possible (NOT PROGRESS RELATED)
3. Make features like when it’s being machined (block/cut)
4. Name useful dimensions and features. Especially when those dimensions are referenced
5. Make several simple features instead of one complicated feature. (More robust and easy to edit)
6. Use fillet features instead of sketch fillets
7. Apply cosmetic fillet and chamfer **last**

## Imported Components

1. Suppress threads
2. When downloading parts, choose the best type available. In order: .sldprt, .sldasm, .igs, .step/stp (AP214), .step (AP203), .stl
3. Complete feature recognition the first time and save. For modified purchased parts, put all original features in a feature folder to make clear what your changes are.
4. For assembly, save as part if you can. If you have to have an imported assembly, put it in a subfolder
5. Try to avoid surface models when possible. Clean up surfaces with the “Delete and Patch” tool.
6. Override mass property with catalog listed mass

## Assembly

1. Origin plane mates (especially first part)
2. If possible, mate all components to one or two fixed references. Long chains of components take longer to solve and more likely to get errors. Do not create loops for mates
3. Fully define the position of each part in assembly, unless visualization of motion needed for certain parts. Option: use mechanical mates.
4. Patterns, not multiple same parts if possible (greatly reduce computing power needed)
5. Lock rotation on cylindrical mate if you don't need rotation.