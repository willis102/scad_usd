# Using Layers and References

## Setup:

1. Unzip `01/assets.zip` into the `01` directory.

## Problem Set:

1. Assemble your shot
    - Open the assembly.usda file and create references to each asset you're interested in using in your shot
    - Try creating multiple references to the same asset and renaming them in your assembled shot.
    - Author this work in the assembly file, and see that the opinions are expressed in the shot stage.

3. Light your shot
    - Copy your lighting.usda file from the previous problem set into this one and see that it's opinions are applied in the shot.  This is pretty cool since they were made in a completely different shot!
    - If you like, author some changes to your lighting (following the same steps as in PS01)

2. Author deltas on your assembly
    - Make a "finishing.usda” file, and add it as the highest subLayer in your shot.
    - Author some deltas to your assembly work in this finishing layer by setting it as the EditTarget, and see that they are expressed in the shot.
    - Open your assembly layer and note that your changes are not expressed here.

3. Make a Shot/Sequence structure with assembly
    - Following the pattern defined in PS01, create a shot/sequence structure in your PS02 work folder.
    - For your sequence USD, swap the old assembly sublayer (assembly.usdc) for the one you made in part 1 of this problem set.
    - Move your finishing sublayer into the shots, and see that this way you can tweak asset placement per-shot by authoring deltas in the shot's finishing layer.
