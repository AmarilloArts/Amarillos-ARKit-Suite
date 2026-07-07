# Amarillo's ARKit Suite

Work in progress. Expect the addon and this readme to get better later.

# What is this?

Amarillo's ARKit Suite is a Blender add-on that adds a controller rig for ARKit face shape keys, so you can drive facial expressions with bones instead of moving the tiny shape key value sliders manually.

# What features does it include?

### Packaged ARKit controller rig

The add-on will append the included `ARKit Controller Rig.blend` collection into your scene, which is just a custom armature.

### ARKit shape key binding

It creates drivers for matching ARKit shape keys on your face mesh. Missing shape keys are skipped, so it only binds what your character actually has. If you already have drivers for those shape keys, you might lose them so plan accordingly.

### Controls

The rig drives a bunch of ARKit shape keys using bones with constraints. At present moment this covers around 60% of shape keys. I'll add more later and I'll expand this section as well.

### Head follow

The controller rig can follow your character's head bone with a `Child Of` constraint, so the face controls move with the head.

### Driver cleanup

You can disable, enable, or remove only the ARKit drivers created by this add-on.

# Use Guide

Install the add-on as usual from the zip file.

After installing, open the panel here:

`3D Viewport > Sidebar > Amarillo > Amarillo's ARKit Suite`

Click `Append Controller Rig` to append the custom armature collection to your scene.

Select your face mesh, or assign it in the `Target Mesh` field. The mesh needs ARKit-style shape keys, such as `eyeBlinkLeft`, `jawOpen`, `mouthSmileLeft`, and so on.

Click `Bind / Refresh Drivers`. The add-on will bind its bones with the matching shape keys using drivers, and optionally make the rig follow your head bone.

If the head follow setup does not find the right bone automatically, assign the character armature in `Head Armature` and type the correct bone name in `Head Bone`.

After binding, pose or animate the controller rig bones to drive the facial shape keys.

# How this addon was made

I am not gonna claim too much credit. I made with by whipping ChatGPT for a few hours with a bunch of instructions. If that makes you not want to use this addon then go ahead and buy yourself an ice cream or something.
