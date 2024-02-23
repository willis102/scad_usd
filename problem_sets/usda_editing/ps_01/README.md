# Edit USDA Manually

## Setup:

1. Unzip `problem_sets/lighting/ps_02/01/assets.zip` into this directory.

## Get familiar with USD by learning to write basic USDA by hand

1. Create a "Hello World" stage
    - Open `hello_world_start.usda` -- you'll see there's a prim called "hello" defined, and nothing more.
    - Define a prim named `/hello/world` by adding a new prim def block inside the "hello" definition.
    - Make `/hello` an `Xform`
    - Make `/hello/world` a `Sphere`

2. Add Attributes
    - Create a `double3` type attribute called `xformOp:translate` on `\hello` and set it to `(0, 10, 0)`
    - Create a `uniform` attribute of type `token[]` called `xformOpOrder` on `\hello` and set it to `["xformOp:translate"]`
    - Reload your stage and see that the Sphere has moved up 10 units
    - Create a `float` type attribute called `radius` on `\hello\world` and set it to `5.0`
    - Reload your stage and see that the Sphere is now sitting on the origin again, but is 10 units across.

3. Add Metadata
    - Set the default prim of your stage to `/hello` by adding `defaultPrim = "hello"` to the layer metadata
    - "Comment out" the `/hello/world` definition block by adding `/**` at the start and `**/` at the end.  This will tell USD to ignore everything between when parsing the file.  Note that if you want to comment a single line, you can use `//` at the beginning of that line, and everything following before the next newline will be ignored.
    - Create a new prim `/hello/book_cover`
    - Add metadata to this prim to make it a reference.  `references = [@./asset/BookVariationA.usdc@]`
    - Upate the reference to load the cover prim from within the Book asset `references = [@./asset/BookVariationA.usdc@</BookVariationA/geo/bookVariation01/bookVariation01_cover>]`

4. If you're feeling really confident, try to follow along with the steps for the lighting Problem Sets editing the files manually.  See how grateful you are for GUIs as you go.
