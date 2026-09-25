<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol~SetSymbol.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSymbol Method (ISFSymbol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISFSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol.html) : SetSymbol Method (ISFSymbol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Symbol*
:   Type of symbol as defined in swSFSymType\_e

*SurfaceTexture*
:   Symbol surface text type as defined in swSFSymType\_e

*AllAround*
:   True if symbol is All Around, false if symbol is Local

Sets the type of symbol for this surface finish symbol.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSymbol( _    ByVal Symbol As System.Integer, _    ByVal SurfaceTexture As System.Integer, _    ByVal AllAround As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISFSymbol Dim Symbol As System.Integer Dim SurfaceTexture As System.Integer Dim AllAround As System.Boolean Dim value As System.Boolean   value = instance.SetSymbol(Symbol, SurfaceTexture, AllAround) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSymbol(     System.int Symbol,    System.int SurfaceTexture,    System.bool AllAround ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSymbol(  &   System.int Symbol, &   System.int SurfaceTexture, &   System.bool AllAround ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Symbol*
:   Type of symbol as defined in swSFSymType\_e

*SurfaceTexture*
:   Symbol surface text type as defined in swSFSymType\_e

*AllAround*
:   True if symbol is All Around, false if symbol is Local

#### Return Value

True if symbol is set, false if it is not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SFSymbol::SetSymbol.

# ![](dotnetimages/collapse.gif)Remarks

The Symbol argument must be one of the following values from the swSFSymType\_e enumeration: swSFBasic, swSFMachining\_Req, swSFDont\_Machine, swSFJIS\_No\_Machining, swSFJIS\_Basic, or swSFJIS\_Machining\_Req.

[ISFSymbol::GetSymbol](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~GetSymbol.html) will get this value.

|  |  |
| --- | --- |
| **If the symbol is...** | **Then...** |
| swSFJIS\_No\_Machining or swSFJIS\_Basic | SurfaceTexture argument must be one of these values from the swSFSymType enumeration: swSFJIS\_Surface\_Texture\_1, swSFJIS\_Surface\_Texture\_2, swSFJIS\_Surface\_Texture\_3, or swSFJIS\_Surface\_Texture\_4.  For any other symbol types, this argument is ignored, and 0 should be passed in. The [ISFSymbol::GetSymbolSurfaceTexture](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~GetSymbolSurfaceTexture.html) method will get this value. |
| swSFBasic, swSFMachining\_Req, or swSFDont\_Machine | AllAround argument indicates whether this is an All Around or Local symbol. Use [ISFSymbol::GetSymbolAllAround](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~GetSymbolAllAround.html) to get this value. |

# ![](dotnetimages/collapse.gif)See Also

####

[ISFSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol.html)

[ISFSymbol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol_members.html)