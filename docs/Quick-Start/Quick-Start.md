# Quick Start

## Installing Unity
The Rude Level Editor is a [Unity](https://unity.com) project which is a modified version of the project Ultrakill was created on. The project contains many [prefabs](https://docs.unity3d.com/2019.4/Documentation/Manual/Prefabs.html), and [scripts](https://docs.unity3d.com/Manual/ScriptingSection.html) which allow you to create a custom level without having much programming knowledge.

To install unity go to [the Official Unity Download](https://unity.com/releases/editor/whats-new/2019.4.40), keep in mind we are download a slightly older version of unity, as Ultrakill runs on `Unity 2019.4.40.f1 (LTS)`.

> [!TIP]
> You can download Unity Hub [here](https://unity.com/download) to manage multiple unity versions and have a better interface when opening projects. 

*Unity's official guide to installing unity is located [here](https://learn.unity.com/tutorial/install-the-unity-hub-and-editor)!* **Make sure to download the correct version!**

## Installing Angry Level Loader

The [Angry Level Loader](https://thunderstore.io/c/ultrakill/p/EternalsTeam/AngryLevelLoader/) is a mod for Ultrakill, and can be installed like any other Ultrakill mod. Below is a video showcasing on how to install mods for Ultrakill, adapt this tutorial to install the Angry Level Loader.


<p style="text-align: center;"><iframe width="750" height="420" src="https://www.youtube.com/embed/rhMKhFNtiNA?si=gD4fHMFTU6gORbg2" title="YouTube video player" frameborder="" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></p>


## Installing Rude Level Editor

Installing the Rude Level Editor is similar to installing any unity project.

Once you arrive in the Rude Discord Server, you will only be able to see the `#rude-gates` channel. Once `@eternalUnion` has given you access to the google drive link download the file.

Then, extract the zip, and import the project into unity. Go to the projects tab and click the small triangle next to `Open`.

![Open project button.](image.png)

Then click `Add project from disk` and locate the project you have just extracted. 

![Add project from disk button.](image-1.png)

> [!PROTIP]
> It's usually good practice to not leave your Unity projects in your download folder. Create a new folder in your disk and move your project there. *(DO THIS BEFORE DOING THE STEP ABOVE!)*

## Linking the Editor to Loader
Open the level exporter window through `Window/Export Level` at the top of the editor.

Press `Open Levels Folder` and select `Ultrakill/BepInEx/plugins/AngryLevelLoader/Levels folder`

When build and copy is pressed, `.angry` files will be copied to the folder

If Ultrakill is **already open** after exporting, press `Reload File` and restart the level

Reloading
If a level is built and copied from rude to angry while Ultrakill is running, the level can be reloaded by pressing "Reload File". If the level was not initially loaded, new levels can be scanned in the root panel

As of **Update 2**, this process can be made with a keybind set through the Angry Level Loader settings. 

---
*Guide Written by: LUKA*
