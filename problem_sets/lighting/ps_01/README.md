# Using Layers

## Setup:

1. Unzip `01/assembly.zip` into the `01` directory.

## Problem Set:

1. Light a single shot that has already been assembled using subLayer and EditTarget
    - Create a “lighting_work.usd” file, and load the assembly and lighting files as subLayers
    - Set the EditTarget of your lighting_work stage to the lighting subLayer
    - Author some work to the lighting subLayer and save it
    - Check that the shot reflects the work you authored work

2. Light shots in a sequence that has already been assembled.  Author a base lighting setup in the sequence, and then author deltas in lighting layers for each shot.
    - Make a “light_rig_work.usd” like you did for #1, but this time for the light_rig.usd file
    - Author base lighting for the sequence in the “light_rig.usd” file using an EditTarget in your light_rig_work file.
    - Now open the lighting_work files for your shots, and using EditTargets on the light layers, author lighting opinions that modify the lighting from the base rig for each shot.
    - You can try changing light transformations, attributes, etc.
