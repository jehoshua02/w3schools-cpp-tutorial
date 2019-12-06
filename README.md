# w3Schools C++ Tutorial Stuff

Tutorial: https://www.w3schools.com/cpp/cpp_getstarted.asp

## Setup

I've committed the configurations (`.vscode`) for how I setup VSCode to build and debug on my macbook.

These are the instructions I followed to generate these configuration files:

https://code.visualstudio.com/docs/cpp/config-clang-mac

I customized the configurations to build and debug the active opened file instead
of a hard coded `helloworld.cpp`.

I found a list of VSCode variables here:

https://code.visualstudio.com/docs/editor/variables-reference

## Build

To build, on macbook in VSCode, open the main file and press `command+shift+B`.

This will generate `.out` and `.out.dSYM` (`.gitignore`'d) files next to the main file, and then
output something like this, in the VSCode integrated Terminal:

```
> Executing task: clang++ -std=c++17 -stdlib=libc++ /Users/joshstoutenburg/projects/w3schools-cpp/00-getting-started/myfirstprogram.cpp -o 00-getting-started/myfirstprogram.out --debug <


Terminal will be reused by tasks, press any key to close it.
```

## Debug

To debug the open active main program file, on macbook in VSCode, hit `fn+F5`.

This will execute the `.out` file and pause at any debugging breakpoints you have
in the source files.