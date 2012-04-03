TiledSharp
==========
A .NET C# library for importing Tiled TMX tile maps

About TiledSharp
----------------
TiledSharp is a C# library for importing TMX tilemaps and TSX tilesets
generated by Tiled, a tile map generation tool. It uses .NET libraries and is
written C#4 syntax. As a generic TMX and TSX parser, TiledSharp does not use
any XNA Game Studio libraries. However, it can be used as a starting point for
XNA game and library development.

Usage
-----
To import a TMX file into your C# application:
- Inclde TiledSharp into your project, either as source or a DLL
- Include the TiledSharp namespace:

    using TiledSharp;
- Create a Map object:

    Map map = new Map("your_file.tmx");

TiledSharp supports both resource names and explicit paths. A detailed
description will be placed in the wiki.

Licensing
---------
I have not yet chosen a license, although I soon plan to release it under
one permitting public use and modification. Please feel free to use or modify
the code as necessary.

Unimplmeneted Features
----------------------
- Recast tile gid array as List, with bit-flipped elements
- Replace `List<e>` with `Dictionary<"name", e>`?
- Testing suite should have a separate project

Contact
-------
Marshall Ward (<marshall.ward@gmail.com>)

Notes
-----

TiledSharp was written to be independent of the XNA Game Studio libraries.
If you are a game developer and seek greater integration with XNA, please
consider Nick Gravelyn's TiledLib.
    
Zlib decompression uses the ZlibStream class of DotNetZip v1.9.1.8.

References
----------

tiled
author: Thorbjørn Lindeijer
web: http://mapeditor.org
dev: https://github.com/bjorn/tiled
    
tiledlib:
author: Nick Gravelyn, Jesse Chounard
dev: https://bitbucket.org/nickgravelyn/tiledlib
    
dotnetzip:
author: Dino Chiesa
dev: http://dotnetzip.codeplex.com
