# Amarillo's ARKit Suite

# What is this?

Amarillo's ARKit Suite is a Blender add-on that adds a controller rig for ARKit face shape keys, so you can drive facial expressions with bones instead of moving sliders manually.

# What features does it include?

### Packaged ARKit controller rig

The add-on can append the included `ARKit Controller Rig.blend` collection into your scene.

### ARKit shape key binding

It creates drivers for matching ARKit shape keys on your face mesh. Missing shape keys are skipped, so it only binds what your character actually has.

### Eye controls

The rig drives eye look, blink, squint, and wide shape keys from the eye guide bones.

### Jaw and mouth controls

It also binds the main jaw, mouth close, smile, frown, dimple, press, stretch, and upper/lower lip controls.

### Head follow

The controller rig can follow your character's head bone with a `Child Of` constraint, so the face controls move with the head.

### Driver cleanup

You can disable, enable, or remove only the ARKit drivers created by this add-on.

# Use Guide

Install the add-on as usual from the zip file.

After installing, open the panel here:

`3D Viewport > Sidebar > Amarillo > Amarillo's ARKit Suite`

Select your face mesh, or assign it in the `Target Mesh` field. The mesh needs ARKit-style shape keys, such as `eyeBlinkLeft`, `jawOpen`, `mouthSmileLeft`, and so on.

If you do not already have the controller rig in the scene, click `Append Controller Rig`.

To set everything up in one step, select or assign the target mesh and click `Bind / Refresh Drivers`. The add-on will append or find the controller rig, bind the matching shape keys, and optionally make the rig follow your head bone.

If the head follow setup does not find the right bone automatically, assign the character armature in `Head Armature` and type the correct bone name in `Head Bone`.

After binding, pose or animate the controller rig bones to drive the facial shape keys.

# How this addon was made

I am actually not very good with python. I made this addon with ChatGPT by asking for what I needed, testing it in Blender, and correcting the parts that were wrong. Make of that what you will.
