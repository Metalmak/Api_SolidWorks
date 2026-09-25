<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateInPlace~MateComponentName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MateComponentName Property (IMateInPlace) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMateInPlace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateInPlace.html) : MateComponentName Property (IMateInPlace) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   0-based index associated with the specified component

Gets the name of the specified component for this **Inplace** mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property MateComponentName( _    ByVal NIndex As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMateInPlace Dim NIndex As System.Integer Dim value As System.String   value = instance.MateComponentName(NIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.string MateComponentName(     System.int NIndex ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ MateComponentName {    System.String^ get(System.int NIndex); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NIndex*
:   0-based index associated with the specified component

#### Property Value

Name of the specified component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MateInPlace::MateComponentName.

# ![](dotnetimages/collapse.gif)Example

[Get Component Names and Types for Inplace MAte (VBA)](Get_Component_Names_and_Types_for_Inplace_Mate_Example_VB.htm)

[Get Mates (C#)](Get_Mates_Example_CSharp.htm)

[Get Mates (VB.NET)](Get_Mates_Example_VBNET.htm)

[Get Mates (VBA)](Get_Mates_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMateInPlace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateInPlace.html)

[IMateInPlace Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateInPlace_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0