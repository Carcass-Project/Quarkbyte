# Quarkbyte

# What is Quarkbyte?
Quarkbyte is a project I am working on that is mostly inspired by raylib, XNA and other graphics frameworks.
It's an OpenTK graphics framework for game-development, but it has other possible uses.
You can have your own shaders, they're written in GLSL.

Quarkbyte supports OpenGL 3.3, but I am planning on changing this to 4.6 in later releases.

# How can I use Quarkbyte?
To use Quarkbyte in your project you can either build the library from the source code here, on Github, or install it through NuGet.
Afterwards create a window and go ham on the drawing functions!

# What does the future hold for Quarkbyte?

Some things that I am planning for Quarkbyte include:
  - [ ] DirectX 11 support.
  - [ ] HLSL shaders through a HLSL to SPIR-V compiler(will need 4.6).
  - [ ] A GUI Library.

But I will also add other things as development goes on, but these are things that I am planning on adding.

# Examples

An example to draw a rectangle on a window would be:
```
using System;
using Quarkbyte;

QWindow = QB.CreateWindow("Example Window - Rectangle", 800,600);

while(!QWindow.Closing)
{
  QB.Clear(Colors.Whiteish);
  QB.DrawRect(5,5,150,150,Colors.Red); // Arguments: X, Y, SizeX, SizeY, Color(enum Colors).
}
  
QWindow.Exit();
```

Other examples are found in the "Examples" folder.
