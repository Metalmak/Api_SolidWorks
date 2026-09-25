<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol~GetSymbolSurfaceTexture.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSymbolSurfaceTexture Method (ISFSymbol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISFSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol.html) : GetSymbolSurfaceTexture Method (ISFSymbol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the symbol surface texture type for this surface finish symbol.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSymbolSurfaceTexture() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISFSymbol Dim value As System.Integer   value = instance.GetSymbolSurfaceTexture() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetSymbolSurfaceTexture() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetSymbolSurfaceTexture(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Symbol surface texture type as defined in swSFSymType\_e (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SFSymbol::GetSymbolSurfaceTexture.

# ![](dotnetimages/collapse.gif)Remarks

[ISFSymbol::GetSymbol](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~GetSymbol.html) returns one of the following values from the swSFSymType\_e enumeration: swSFBasic, swSFMachining\_Req, swSFDont\_Machine, swSFJIS\_No\_Machining, swSFJIS\_Basic, or swSFJIS\_Machining\_Req.

|  |  |
| --- | --- |
| **If the symbol is...** | **Then use...** |
| swSFJIS\_No\_Machining or swSFJIS\_Basic | ISFSymbol::GetSymbolSurfaceTexture to retrieve more information about the symbol.    It returns one of these values from the swSFSymType\_e enumeration: swSFJIS\_Surface\_Texture\_1, swSFJIS\_Surface\_Texture\_2, swSFJIS\_Surface\_Texture\_3, or swSFJIS\_Surface\_Texture\_4. |
| swSFBasic, swSFMachining\_Req, or swSFDont\_Machine | [ISFSymbol::GetSymbolAllAround](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~GetSymbolAllAround.html) to retrieve more information about the symbol. This method returns a Boolean indicating whether this is an All Around or Local symbol. |

To set the symbol type, use [ISFSymbol::SetSymbol](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISFSymbol~SetSymbol.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISFSymbol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol.html)

[ISFSymbol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISFSymbol_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0