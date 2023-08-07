# C# .NET Wrapper for the Open Asset Import Library (Assimp)

Since Google Code no longer allows new downloads, the latest release can be downloaded via NuGet or on this side.

A .NET wrapper for the Open Asset Import Library (Assimp). The wrapper uses P/Invoke to communicate with Assimp's C-API and is divided into two parts:

Low-level
The native methods are exposed via the AssimpLibrary singleton.
"Unmanaged" structures prefixed with the name 'Ai' that contain IntPtrs to the unmanaged data.
The unmanaged library is loaded/unloaded dynamically, 32 and 64 bit is supported. The managed DLL is 'AnyCPU'
Located in the 'Assimp.Unmanaged' namespace.
High-level
A more C# like interface that is more familiar to .NET programmers and allows you to work with the data in managed memory.
Completely handles data marshaling for both import and export, the user left only concerned with the data itself.
Located in the default 'Assimp' namespace.
The High level layer is very similar to Assimp's C++ API and the low level part is public to allow users do whatever they want (e.g. maybe load the unmanaged data directly into their own structures).

For a brief overview and code sample, check out the Getting Started wiki page.

The binaries were built in Visual Studio 2012 as AnyCpu and target .NET 4.5 and .NET 2.0. They are deployed with the Assimp 3.1.1 release (you can download the latest Assimp releases here).

Enjoy!

In addition, check out these other projects from the same author:

Tesla Graphics Engine - a 3D rendering platform written in C# and the primary motivation for developing AssimpNet.
DevIL.NET - a sister C# wrapper for the Developer Image Library (DevIL). (Mostly a relic at this point)
Follow project updates and more on Twitter

A support forum is located here. Feel free to post questions or comments on the direction of the library
