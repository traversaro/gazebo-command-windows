# gazebo-command-windows
gazebo command for the versions of the Gazebo simulator that on Windows does not provide it.

Up to Gazebo 11.2, all the version of Gazebo availale on Windows provide the two separate binaries `gzserver` and `gzclient`, 
but do not provide the unified command `gazebo` that is commonly used by users and in documentation and examples. This repo provide
the `gazebo` command also on Windows.

## Build 
Compile Gazebo for Windows or download a Gazebo binary build, for example from https://github.com/robotology/robotology-superbuild-dependencies-vcpkg .

Then, download, compile and install this repo:
~~~
git clone https://github.com/traversaro/gazebo-command-windows
cd gazebo-command-windows
cmake -DCMAKE_INSTALL_PREFIX=<install_prefix>
cmake --build . --config Release
cmake --install . --config Release
~~~

## Use 
To use the binary, either add `<install_prefix>/bin` to the path and then launch the `gazebo` command from terminal.

![gazebo_command_windows](https://user-images.githubusercontent.com/1857049/97082362-4c90b200-1609-11eb-9ea4-79a331ba4638.gif)

