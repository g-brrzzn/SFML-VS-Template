# SFML Template for Visual Studio  

This repository contains a fully configured Visual Studio project for SFML, following the official guide:  
🔗 [SFML Setup Guide for Visual Studio](https://www.sfml-dev.org/tutorials/3.0/getting-started/visual-studio/)  

## Configuration  

Before using this template, update the project properties to match your SFML installation path:  

- **Project's properties -> C/C++ > General > Additional Include Directories**  
  Change to the path where your SFML headers are located (currently set to `"D:\libs\SFML-3.0.0\include"`).  
- **Project's properties -> Linker > General > Additional Library Directories**  
  Change to the path where your SFML libraries are located (currently set to `"D:\libs\SFML-3.0.0\lib"`).  

## Project Settings  

The following configurations are already set up in this template:  

- **Project's properties -> C/C++ > Language > C++ Language Standard >** "ISO C++ 17 Standard"  
- **Project's properties -> C/C++ > General > Additional Include Directories >** "<sfml-install-path>/include"  
- **Project's properties -> Linker > General > Additional Library Directories >** "<sfml-install-path>/lib"  
- **Project's properties -> Linker > Input > Additional Dependencies >** Added `"sfml-graphics.lib"`, `"sfml-window.lib"`, and `"sfml-system.lib"`  
- **Project's properties -> Preprocessor Definitions >** Added `"SFML_STATIC"` (for static linking)  
- **Project's properties -> Linker > Input > Additional Dependencies >** Added additional libraries for static linking, such as `"opengl32.lib"`, `"winmm.lib"`, `"gdi32.lib"`, `"freetype.lib"`, `"flac.lib"`, `"vorbisenc.lib"`, `"vorbisfile.lib"`, `"vorbis.lib"`, `"ogg.lib"`, `"ws2_32.lib"` (depending on the SFML module used)  
- **Project's properties -> Linker > Input > Additional Dependencies >** Added `"sfml-main-d.lib"` (Debug) or `"sfml-main.lib"` (Release) for "Windows application" projects  

## Creating a Project Template  

To save this project as a reusable template in Visual Studio:  

1. Open **Visual Studio**.  
2. Go to the **Project** menu and select **Export Template...**.  
3. Choose **Project Template**, then click **Next**.  
4. Select this SFML project from the list.  
5. Fill in the template name and description.  
6. Click **Finish**.  

## Download
📥 **Download SFML**: [SFML Official Download Page](https://www.sfml-dev.org/download/)  
📂 Installation Instructions:
Download the SFML SDK (ZIP file) and extract it to your preferred location. The extracted folder will be named SFML-3.0.0 (or the version you downloaded). Use this folder's include and lib directories when configuring the project in **Configuration** section.
