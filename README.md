# Hololens 2 Unity tutorial (Windows)

[1. Setup and first build](#setup)

## <a name="setup"></a>Setup and first build
In this section, I'll be teaching you how I got my first project up and running in Hololens 2, from an application built in Unity.

### First part - installing packages and applications
1. Let's start by installing Visual Studio Community 2022, in case you don't have it yet. [Here](https://visualstudio.microsoft.com/downloads/) you can find the microsoft page to install it. Wheater you donwloaded it just now or already had VS on your machine, be sure to add the following workloads on your installation: (You can have access to that if you go to Settings -> System -> Storage -> Apps & Features, then search for Microsoft Visual Studio Installer, click Modify and then Modify again.
    * .NET desktop development (or download manually [here](https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/runtime-desktop-5.0.16-windows-x64-installer))
    * Desktop development with C++
    * Universal Windows Platform (UWP) development
    * Game development with Unity

2. Now, if you don't have the Windows 10 SDK, you can find the installer [here](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/)
3. Download the Emulator [here](https://go.microsoft.com/fwlink/?linkid=2193111) (opitional, just in case you don't have the Hololens in hand)
4. Open Unity Hub and install the Universal Windows Platform Build Support module for the unity version that you want to use (unity 2019.3 not recomended due to compile errors in ARM build architecture). You can do that by opening unity hub -> Installs -> clicking the gear button for the version you want -> Add Modules -> Universal Windows Platform Build Support.
