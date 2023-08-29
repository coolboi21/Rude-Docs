# FAQ

**Welcome to the Rude Level Editor FAQ.**

Please keep in mind that this page is always being updated!

## Frequently Asked Questions

### Help! Some of my objects turned pink! :space_invader: 
While this this can be caused by many things, what pink usually means is that the material you assigned to your gameobject has a missing texture.
This can be caused by:
- Deleting a texture asset a material uses
- Using textures from premade Ultrakill assets, instead of assigning a gameobject the material that texture corresponds too. 
- (Very Unlikely) Shaders used are not supported by the Unity's current render pipline, the [Built-In Render Pipeline](https://docs.unity3d.com/2019.4/Documentation/Manual/built-in-render-pipeline.html).

### MY CHECKPOINTS ARENT WORKING WHYYYYYYYYY!!! :sob::sob::sob::sob:
This also can be caused by many things, just make sure your checkpoints follow the rules below:
- **Checkpoints must not have a parent!**
- Remember the room you want to save the progress of should be referenced under `Rooms To Inherit`

![checkpoint component](assets/checkpoint-rooms-to-inherit.png)
- The room that should be activated on respawning at the checkpoint should be referenced under `To Activate`

### Why aren't my custom scripts working? :floppy_disk:
Remember while developing for Ultrakill, you can't use all of Unity's functionalities including created scripts as usual.
Here are some things to watch out for:
- To create custom scripts for your level follow [this guide](/Tutorials/Advanced/Custom%20Scripting.md).
- If you modified your `.dll` in your Ultrakill's `Scripts` folder remember to restart the game.
- Make sure to import your `.dll` into your project's `RudeScripts` an no where else.

### How do I get access to the Rude Level Editor??

[here](https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab_channel=RickAstley "Rude Download (Official)") :expressionless:

---
*Page Written by: LUKA*
