## Godot-cpp template
This is a very basic template for Godot 4.4 for C++.

## Contents
- godot-cpp (-b 4.4) repo as a sub-module
- Empty godot project
- include directory for project headers
- src directory for the code (has a basic register_types.cpp for binding classes)
- SCons (requires python) file for building

## How to use the template

## Things to know
1. The temporary name used is 'NEXTGAME', which is used for .gdextension file name, all linked libraries, and the entry symbol used for
initiliasing the module (entry symbol is in .gdextension file and the method in `src/register_types.cpp`).

2. By default, 'compile_commands.json' is always generated (can be changed in `SConstruct`).

3. By default, if `scons` command is used, your current platform is used for building. Can specify using `platform=<OS>`.

Find more info, and see the example on Godot online documentation.
[GDExtension(C++) - docs](https://docs.godotengine.org/en/stable/tutorials/scripting/gdextension/gdextension_cpp_example.html)
