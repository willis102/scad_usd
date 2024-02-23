# Edit USDA Manually
## Get familiar with USD by learning to write basic USDA by hand

For this second problem set, we'll make a simple "tree" asset using GPrims

- Open `tree_start.usda` -- you'll see there's already a default prim at the root called `Tree`
- Define a prim with IsA schema `Cone` named `/Tree/Foliage_01` by adding a new prim def block inside the `Tree` definition.
- Create attributes for your Cone so that it points up along the Y-axis and you can set its dimensions:
    - `uniform token axis = "Y"`
    - `double height = 100`
    - `double radius = 50`
- Open your tree USD file, and you should see your cone.
- Create two more `Cone` prims as children of `Tree`, `Foliage_02` and `Foliage_03`
- Add a translate xform to these, like you did in ps_01.
- Scale and position your three cones so that each is offset upwards along the y-axis, and decreases in scale, to give the approximate appearance of a tree.
- Finally, add one more prim, with IsA schema `Cylinder`, and call it `Trunk`.  This schema can be controlled with the same three attributes as our Cone.
- Set the dimensions and add a translation so that this cylinder looks like a trunk coming out of the bottom of your tree.
- Admire your work

- Extra Credit:
    - Organize the hierarchy of this asset better, and transform your work so that the Tree sits on the origin.
    - Try and do this without transforming the `defaultPrim` -- remember that those transformations won't be useful if we `Reference` our tree.
