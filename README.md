# SDL Example

This project will show how to setup a project with SDL graphic library and CMake.

## Installation

### Ubuntu

1. Install library for development:

```shell script
sudo apt install libsdl2-dev 
```

2. Add these lines to your cmake list file ( ```CmakeLists.txt``` ):
~~~cmake
find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

target_link_libraries(sdltest ${SDL2_LIBRARIES})
~~~

**Note**: `sdltest` is the name of your project and you should replace it with a proper name that is defined in your cmake file.