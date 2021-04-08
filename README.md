```
     _____ _______ ______             _            
    / ____|__   __|  ____|           (_)           
   | (___    | |  | |__   _ __   __ _ _ _ __   ___ 
    \___ \   | |  |  __| | '_ \ / _` | | '_ \ / _ \
    ____) |  | |  | |____| | | | (_| | | | | |  __/
   |_____/   |_|  |______|_| |_|\__, |_|_| |_|\___|
                                 __/ |               
                                                          
```   

## Why prepare this tutorials ？

> During this period of time, I have been sorting out the OpenGL and DirectX11 tutorials, and there has been no time to finish. In the process, I have an idea to build a cross-platform rendering engine from scratch, so let's start!

## Environment
- VS Code Version 1.53
- Visual Studio 2019
- Tree Version 1.7.0
- CMake Version 3.19.0
- System Windows 10 & Ubuntu 18.04.2 GNU/Linux 

## Introduction
> The engine should first include two parts of **Runtime** and **Editor**, and secondly, it should include third-party libraries and platform layer. First, we establish the file structure for the engine. We will start with **Runtime** and iterate step by step.

## Include

```console
PS D:\Workspace\private\STEngine> tree .
D:.
├─Editor
├─External
├─Platforms
│  ├─Android
│  ├─iOS
│  ├─Linux
│  ├─OSX
│  └─Windows
└─Runtime
    ├─Allocator
    ├─Application
    ├─Camera
    ├─GfxDevice
    │  ├─d3d11
    │  ├─d3d12
    │  ├─metal
    │  ├─null
    │  ├─opengl
    │  ├─opengles
    │  └─vulkan
    ├─Input
    ├─Interfaces
    ├─Network
    ├─Profiler
    └─Resources
```

## Supported Platforms
- Microsoft Windows
- Apple macOS
- Linux
- Android
- iOS
