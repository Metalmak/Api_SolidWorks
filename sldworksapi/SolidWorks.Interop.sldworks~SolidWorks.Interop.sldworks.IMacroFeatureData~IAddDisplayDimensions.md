<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IAddDisplayDimensions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddDisplayDimensions Method (IMacroFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html) : IAddDisplayDimensions Method (IMacroFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DimCount*
:   Number of display dimensions

*DimTypes*
:   * in-process, unmanaged C++: Pointer to an array of display dimension types as defined swDimensionType\_e* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*DimValues*
:   * in-process, unmanaged C++: Pointer to an array of display dimension values* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Adds the specified display dimensions to this macro feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IAddDisplayDimensions( _    ByVal DimCount As System.Integer, _    ByRef DimTypes As System.Integer, _    ByRef DimValues As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData Dim DimCount As System.Integer Dim DimTypes As System.Integer Dim DimValues As System.Double   instance.IAddDisplayDimensions(DimCount, DimTypes, DimValues) ``` | |

| C# |  |
| --- | --- |
| ``` void IAddDisplayDimensions(     System.int DimCount,    ref System.int DimTypes,    ref System.double DimValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IAddDisplayDimensions(  &   System.int DimCount, &   System.int% DimTypes, &   System.double% DimValues ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DimCount*
:   Number of display dimensions

*DimTypes*
:   * in-process, unmanaged C++: Pointer to an array of display dimension types as defined swDimensionType\_e* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*DimValues*
:   * in-process, unmanaged C++: Pointer to an array of display dimension values* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0