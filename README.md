# VS Launcher (VSL)

Visual Studio Launcher (VSL) is a WPF program in the VS Tools suite that allows you to open Visual Studio solutions and other files in a specified version of Visual Studio. Designed with a Visual Studio-like interface, VSL supports both dark and light themes, integrating seamlessly into your development workflow.

### Key Features

- **Compatibility**: Supports Visual Studio versions that use the native installer.
- **Save File Version**: Option to remember your preferred Visual Studio version for each solution.
- **Command-Line Integration**: Open solutions directly from the command line, and optionally with a specified version.
- **Design**: Interface design similar to Visual Studio, made in WPF.
- ```Coming Soon``` **Custom Splash Screen**: Choose a custom splash screen when Visual Studio opens.
- ```Coming Soon``` **Themes**: Create your own themes to match your workflow.

### Installation

**Software Requirements**:
- .NET Desktop 8.
- Supports all Visual Studio versions from 2019.

**Installation Steps**:
1. Download the [latest release](https://github.com/polylogue2/vs-launcher/releases/latest) of VSLSetup.exe.
2. Launch the downloaded executable.
3. Follow the installation prompts. During the installation, you will have options to:
   - Register file associations automatically. (default .SLN)
   - Add "Open with VSL" to the context menu.
4. After installation, you can load VS Launcher.

### Usage

**1. Opening Files**
When you load a `.sln` file, VSL will prompt you to choose a version of Visual Studio to open it with. If only one version is installed, it will automatically open the solution with that version. This can be changed in settings

**2. Settings**
The settings page can be accessed on top of the window, next to the close button. From here, you can change themes, edit saved version configuration, and other additional settings.

**3. Using Command Line**
You can launch VSL from the command line by specifying the path to a file, and other parameters listed below:
- **--version** Specify an installed version to load the file
- **--admin** Launches the solution as an administrator

````
vsl.exe "C:\dev\helloworld.sln" --version 2022_community --admin
````
*This command will open the specified solution using Visual Studio 2022 Community Edition with administrative privileges.*
