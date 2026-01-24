# Building For Windows

This page breaks down the steps for building for Windows.

## Prerequisites

### Visual Studio
[Visual Studio](https://visualstudio.microsoft.com/downloads/) is the standard IDE for Windows development. 
Whilst its not the only option it is the most tested and supported for the engine.

Currently there are the supported versions of Visual Studio:
* Visual Studio 2022 64-bit
* Visual Studio 2026 64-bit

These workloads have to be installed:
* Desktop Development with C++
* Game Development with C++
* .Net Desktop Development

## Generating the Project Files
### Build Scripts
in the root of the repository you will find some <path>.bat</path> files, such as:
- <path>GenerateWin64vs2022.bat</path>
- <path>GenerateWin64vs2026.bat</path>

Run one of them to generate a Visual Studio solution for your preferred compiler. Afterwards, there will be a Workspace folder in the root folder, where you find a PlasmaEngine2_***.sln file in the respective folder for the Visual Studio version that you chose.

> **Note:** </br>
> Visual Studio 2026 uses the new .slnx solution file format. If double-clicking the .slnx file opens it in Visual Studio 2022 instead of 2026, you need to adjust your Windows file association settings to ensure .slnx files open with the correct Visual Studio version.
{style="note"}

If the script fails, you most likely don't have all the prerequisites installed. They also sometimes fail, if Visual Studio recently installed an update and you haven't rebooted your PC since. Usually when this script fails it is due to common issues with CMake or the MSVC installation. Read the full error messages carefully and search the internet, you'll usually find a solution quickly.

### Manually via CMake
This path requires you to install [CMake](https://cmake.org/) yourself. CMake allows you to enable optional features that are not enabled by default.

Run the CMake GUI and configure the build options.

> **Important:** </br>
> If you are new to C++ or CMake we recommend using the build scripts. since this will cover many of the setup pitfalls.
> {style="note"}

## Building
Open the generated solution with Visual Studio and build everything. Run the Editor project afterwards.

## See Also
* [Building Plasma](Building-Plasma.md)