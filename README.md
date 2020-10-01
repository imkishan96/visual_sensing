# visual_sensing

## Required libraries


## install
download and bootstrap vcpkg if you havent already
```
> git clone https://github.com/microsoft/vcpkg
```
checkout older tag 2020.04 because of compatibilty of pcl with VTK 9.0 is not yet available
```
> cd vcpkg
> .\bootstrap-vcpkg.bat
> .\vcpkg integrate install
```
last command `.\vcpkg integrate install` will provide the cmake tool chain path `-DCMAKE_TOOLCHAIN_FILE=[path to vcpkg]/scripts/buildsystems/vcpkg.cmake` save it for later use

install pcl 
```
> .\vcpkg install pcl 
```
install realsense2
```
> .\vcpkg install realsense2
```
clone this repo
```
> git clone https://github.com/imkishan96/visual_sensing.git
```
setup the workspace setting for CMake tool chain on vscode press `ctrl + shift + p`   serach preferences:Open Workspace Settings and
add previously saved cmake tool chain path to the setting file 
`"CMAKE_TOOLCHAIN_FILE":'[path to vcpkg]/scripts/buildsystems/vcpkg.cmake'`