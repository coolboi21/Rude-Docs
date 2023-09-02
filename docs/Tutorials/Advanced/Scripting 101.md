# Scripting 101 (Advanced Tutorial)

This will teach you how to set up a Visual Studio project for Ultrakill [custom script making](https://docs.unity3d.com/2019.4/Documentation/Manual/ScriptingSection.html). 

## Prerequisites
- [**Visual Studio**](), prefebally version 2022.
- **Bepinex Templates**. If not installed, `run dotnet new -i BepInEx.Templates` `--nuget-source https://nuget.bepinex.dev/v3/index.json` from command line.
- **Bepinex Nuget Source**. Run `dotnet nuget add source https://nuget.bepinex.dev/v3/index.json --name Bepinex` just in case

## Insalling the Template
Download the template below to get started.

[Ultrakill Scripting Template](../../../../../../Users/coolboi_21/Downloads/UltrakillProject.zip)

Put the template in `C:\Users\{Your User Name}\Documents\Visual Studio 2022\Templates\ProjectTemplates`

Restart Visual Studio if it is open.

## Creating the Project

Create a new project using the template `UltrakillProject`. Reset search filters if it is not there.

Write your scripts. Compile with Ctrl + Shift + B

Copy the `.dll` in bin folder to `YourRudeProject/Assets/RudeScripts` and `Angry/Scripts` (*it is important that the script is in the `RudeScripts` folder for the level exporter to detect the components as custom scripts*)

## Script Certificates

### What is a Script Certificate <!-- {docsify-ignore} -->
Script certificate, of format `.dll.cert` is a file containing [`sha256 hash`](https://www.simplilearn.com/tutorials/cyber-security-tutorial/sha-256-algorithm) of the script file signed with the angry loader private key. The script can be verified on angry side by decrypting the certificate with the public key and comparing it with the file hash. This means that when the dll content is changed, certificate will no longer match the file.

---

### How to get a script certificate <!-- {docsify-ignore} -->
Send the file to `@eternalUnion`, they will check its content. If it is not a malicious script they will send the certificate back. The script can also be uploaded online for angry to download if your level depends on it.

## Known Problems
Custom scripting for the Rude Level Editor has some limitations, listed below:

- Do not use Bepinex types as fields (*even if static*) in unity scripts (like `MonoBehavior` or `ScriptableObject`). 
> [!TIP]
> To use Bepinex types put them in another class instead. 
>
>For example, if you want to patch a method create a static method to contain the Harmony object and patch methods

- Do not derive from `UnityPlugin`.


## Conclusion
Now you can get started creating custom scripts to bring your Ultrakill levels to... the next level!

Maybe even follow the [enemy creation tutorial]() to learn how to create your own custom enemies!

## Useful Resources

* [Scripting in Unity (Unity Docs)](https://docs.unity3d.com/2019.4/Documentation/Manual/ScriptingSection.html)
* [Visual Studio (Download)](https://visualstudio.microsoft.com)
* [In-Depth SHA 256 Explanation](https://www.simplilearn.com/tutorials/cyber-security-tutorial/sha-256-algorithm)

---

*Guide Written by: eternalUnion*

*Adapted & Expanded by: LUKA*

