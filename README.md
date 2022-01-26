# Croak
Custom Source Engine branch based on Source Engine 2007, currently available on Windows in x86.

Based on <a href="https://github.com/quiverteam/Engine">Quiver</a>.

**Pull this repository with recursive submodules (`git clone --recursive`) to clone qpc and game/core folder**

## Building

### Windows

1. Install [Visual Studio 2019+](https://visualstudio.microsoft.com/downloads/), Make sure to go to Individual components and install `C++ MFC for v142 build tools (x86 and x64)`

2. Install [Python](https://www.python.org/downloads/), 3.6+, and make sure to check the "py launcher" option when installing

3. Run src/\_create\_allprojects.bat

4. Open the solution created, build "Game" in Release Win32, or alternatively the entire solution if wanted.

#### OPTIONAL - Building Shaders:

1. Install [Perl](http://strawberryperl.com/), open Perl Command Line and enter `cpan String::CRC32`.

2. (Only if you didn't build shadercompile and dx\_proxy yet) Run src/\_create_coreprojects.bat and build the solution in Release - Win32.

3. Build shaders by running src/materialsystem/stdshaders/\_buildallshaders.bat.

4. Build stdshader_xxx projects in Visual Studio again.

### Linux and MacOS

Linux and MacOS support is currently being worked on in the posix-support branch. If you want to help, See Supporting Non-Windows Platforms.

## Running the Game

### Windows
1. Edit game/make_dir_junction.bat with your HL2 install directory if needed and run.
2. Run the game with any one of the game/run\_mod\_x.bat files

### Links
