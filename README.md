# Hololens 2 Unity tutorial (Windows)

[1. Setup and first build](#setup)

## <a name="setup"></a>Setup and first build
In this section, I'll be teaching you how I got my first project up and running in Hololens 2, from an application built in Unity.

### First step - installing packages and applications
1. Let's start by installing Visual Studio Community 2022, in case you don't have it yet. [Here](https://visualstudio.microsoft.com/downloads/) you can find the microsoft page to install it. Wheater you donwloaded it just now or already had VS on your machine, be sure to add the following workloads on your installation: (You can have access to that if you go to Settings -> System -> Storage -> Apps & Features, then search for Microsoft Visual Studio Installer, click Modify and then Modify again.
    * .NET desktop development (or download manually [here](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-5.0.16-windows-x64-installer)).
    * Desktop development with C++.
    * Universal Windows Platform (UWP) development.
    * Game development with Unity.
2. Now, if you don't have the Windows 10 SDK, you can find the installer [here](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/).
3. Download the Emulator [here](https://go.microsoft.com/fwlink/?linkid=2193111) (opitional, just in case you don't have the Hololens in hand).
4. Open Unity Hub and install the Universal Windows Platform Build Support module for the unity version that you want to use (unity 2019.3 not recomended due to compile errors in ARM build architecture). You can do that by opening unity hub -> Installs -> clicking the gear button for the version you want -> Add Modules -> Universal Windows Platform Build Support.
5. Last but not least, install the Mixed Reality Feature Tool from Microsoft [here](https://www.microsoft.com/en-us/download/details.aspx?id=102778).

We're all set, now it's time to build our first application!

### Second step - creating first unity project
1. Open Unity Hub.
2. In the Projects tab, click New Project.
3. In the dropdown underneath the New project text, select the unity version that you have installed Universal Windows Platform Build Support.
4. The template must be 3D Core.
5. Click Create Project.

### Third step - configuring build for Hololens 2
1. Go to File -> Build Settings
2. Select Universal Windows Platform.
3. Click Switch Platform if needed.
4. Now make sure to set the following settings: (if any error occurs, check if all the instalations are properly working)
      * Target device: HoloLens
      * Architecture: ARM64
      * Build Type: D3D Project
      * Target SDK Version: Latest Installed
      * Minimum Platform Version: 10.0.10240.0
      * Visual Studio Version: Latest installed
      * Build and Run on: Local Machine
      * Build configuration: Release (there are known performance issues with Debug)

### Forth step - importing and configuring MKT in Unity
1. Open the previously installed Mixed Reality Feature Tool, and run MixedRealityFeatureTool.exe (unzip the folder if necessary).
2. In the Mixed Reality Feature Tool, select Start.
3. Select the project foldr that we've created by clicking the three dots in Project Path.
4. Click Discover Features.
5. On the Discover Features page click the "+" button to the left of Mixed Reality Toolkit (0 of 10) and select the latest version of Mixed Reality Toolkit Foundation.
6. On the Discover Features page Click the "+" button to the left of Platform Support (0 of 5) and select the latest version of Mixed Reality OpenXR Plugin.
7. Click Get Features.
