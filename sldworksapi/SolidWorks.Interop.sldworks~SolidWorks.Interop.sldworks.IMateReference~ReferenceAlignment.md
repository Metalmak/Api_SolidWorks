<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference~ReferenceAlignment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReferenceAlignment Property (IMateReference) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMateReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference.html) : ReferenceAlignment Property (IMateReference) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Mate reference entity as defined by swMateReferenceIndex\_e

Gets the mate reference alignment for the specified mate reference entity in the selected mate reference.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ReferenceAlignment( _    ByVal Index As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMateReference Dim Index As System.Integer Dim value As System.Integer   value = instance.ReferenceAlignment(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ReferenceAlignment(     System.int Index ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int ReferenceAlignment {    System.int get(System.int Index); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Mate reference entity as defined by swMateReferenceIndex\_e

#### Property Value

Type of alignment as defined by swMateReferenceAlignment\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MateReference::ReferenceAlignment.

# ![](dotnetimages/collapse.gif)Example

[Get Mate Reference Properties (VBA)](Get_Mate_Reference_Properties_Example_VB.htm)

[Get Mate Reference Properties (VB.NET)](Get_Mate_Reference_Properties_Example_VBNET.htm)

[Get Mate Reference Properties (C#)](Get_Mate_Reference_Properties_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this property, call [IMateReference::ReferenceEntityCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMateReference~ReferenceEntityCount.html) to determine the number of mate reference entities for the mate reference.

This method returns -1 if there is no reference entity. See [IMateReference::ReferenceEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMateReference~ReferenceEntity.html) for details.

# ![](dotnetimages/collapse.gif)See Also

####

[IMateReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference.html)

[IMateReference Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0