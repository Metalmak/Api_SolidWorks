<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateLoadReference~GetFacesCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFacesCount Method (IMateLoadReference) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMateLoadReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateLoadReference.html) : GetFacesCount Method (IMateLoadReference) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WhichOne*
:   * 0 = Component1* 1 = Component2

Gets the number of supplemental faces of the mate associated with the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFacesCount( _    ByVal WhichOne As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMateLoadReference Dim WhichOne As System.Integer Dim value As System.Integer   value = instance.GetFacesCount(WhichOne) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetFacesCount(     System.int WhichOne ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetFacesCount(  &   System.int WhichOne ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WhichOne*
:   * 0 = Component1* 1 = Component2

#### Return Value

Number of supplemental faces of the mate associated with the specified component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MateLoadReference::GetFacesCount.

# ![](dotnetimages/collapse.gif)Example

[Insert Mate Load Reference (C#)](Insert_Mate_Load_Reference_Example_CSharp.htm)

[Insert Mate Load Reference (VB.NET)](Insert_Mate_Load_Reference_Example_VBNET.htm)

[Insert Mate Load Reference (VBA)](Insert_Mate_Load_Reference_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The supplemental faces can belong to one of two components. Specify the component that owns the supplemental faces that you want to access.

Call this method before calling [IMateLoadReference::IGetFaces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMateLoadReference~IGetFaces.html) to determine the size of the array.

# ![](dotnetimages/collapse.gif)See Also

####

[IMateLoadReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateLoadReference.html)

[IMateLoadReference Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateLoadReference_members.html)

[IMateLoadReference::GetFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateLoadReference~GetFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0