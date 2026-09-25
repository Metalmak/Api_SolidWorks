<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertCavity4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCavity4 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : InsertCavity4 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ScaleFactor\_x*
:   Scaling factor in the x direction

*ScaleFactor\_y*
:   Scaling factor in the y direction

*ScaleFactor\_z*
:   Scaling factor in the z direction

*IsUniform*
:   True to use the first scale argument as the uniform scale, false to not

*ScaleType*
:   Type of scaling as defined in swCavityScaleType\_e

*KeepPieceIndex*
:   Piece to keep if there is ambiguity

Inserts a cavity to the active part using a selected component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertCavity4( _    ByVal ScaleFactor_x As System.Double, _    ByVal ScaleFactor_y As System.Double, _    ByVal ScaleFactor_z As System.Double, _    ByVal IsUniform As System.Boolean, _    ByVal ScaleType As System.Integer, _    ByVal KeepPieceIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim ScaleFactor_x As System.Double Dim ScaleFactor_y As System.Double Dim ScaleFactor_z As System.Double Dim IsUniform As System.Boolean Dim ScaleType As System.Integer Dim KeepPieceIndex As System.Integer   instance.InsertCavity4(ScaleFactor_x, ScaleFactor_y, ScaleFactor_z, IsUniform, ScaleType, KeepPieceIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertCavity4(     System.double ScaleFactor_x,    System.double ScaleFactor_y,    System.double ScaleFactor_z,    System.bool IsUniform,    System.int ScaleType,    System.int KeepPieceIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertCavity4(  &   System.double ScaleFactor_x, &   System.double ScaleFactor_y, &   System.double ScaleFactor_z, &   System.bool IsUniform, &   System.int ScaleType, &   System.int KeepPieceIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ScaleFactor\_x*
:   Scaling factor in the x direction

*ScaleFactor\_y*
:   Scaling factor in the y direction

*ScaleFactor\_z*
:   Scaling factor in the z direction

*IsUniform*
:   True to use the first scale argument as the uniform scale, false to not

*ScaleType*
:   Type of scaling as defined in swCavityScaleType\_e

*KeepPieceIndex*
:   Piece to keep if there is ambiguity

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::InsertCavity4.

# ![](dotnetimages/collapse.gif)Example

[Insert Cavity (C#)](Insert_Cavity_Example_CSharp.htm)

[Insert Cavity (VB.NET)](Insert_Cavity_Example_VBNET.htm)

[Insert Cavity (VBA)](Insert_Cavity_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This operation is performed in the context of an assembly document. The component being edited in the context of the assembly receives the new cavity feature.

Set the scaleFactor argument as appropriate for your casting material. The scaling factor is expressed as a percentage (+/- 20%) of the size of the cavity part. Pass it in as a value within the range of -20 to +20.

SOLIDWORKS uses the following formula to determine the size of the cavity:

cavitysize = partsize \* (1 + scaleFactor/100)

When there is ambiguity in the result of a cut, SOLIDWORKS uses KeepPieceIndex to determine which result to use. You can set this parameter to -1 if there is no ambiguity; otherwise, you should use the index of the result, in the range between 0 and 1 less than the possible number of outcomes.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[ICavityFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICavityFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0