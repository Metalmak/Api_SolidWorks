<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ImportDiagnosisGapCloser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImportDiagnosisGapCloser Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : ImportDiagnosisGapCloser Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OldX*
:   x coordinate of vertex to move

*OldY*
:   y coordinate of vertex to move

*OldZ*
:   z coordinate of vertex to move

*NewX*
:   x coordinate where to move the vertex

*NewY*
:   y coordinate where to move the vertex

*NewZ*
:   z coordinate where to move the vertex

*LastMove*
:   True if this move is the last move in a series of moves to close the gap, false if not

Allows you to repair a gap by moving the vertices on the edges surrounding the gap to new positions to close the gap on the imported model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ImportDiagnosisGapCloser( _    ByVal OldX As System.Double, _    ByVal OldY As System.Double, _    ByVal OldZ As System.Double, _    ByVal NewX As System.Double, _    ByVal NewY As System.Double, _    ByVal NewZ As System.Double, _    ByVal LastMove As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim OldX As System.Double Dim OldY As System.Double Dim OldZ As System.Double Dim NewX As System.Double Dim NewY As System.Double Dim NewZ As System.Double Dim LastMove As System.Boolean   instance.ImportDiagnosisGapCloser(OldX, OldY, OldZ, NewX, NewY, NewZ, LastMove) ``` | |

| C# |  |
| --- | --- |
| ``` void ImportDiagnosisGapCloser(     System.double OldX,    System.double OldY,    System.double OldZ,    System.double NewX,    System.double NewY,    System.double NewZ,    System.bool LastMove ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ImportDiagnosisGapCloser(  &   System.double OldX, &   System.double OldY, &   System.double OldZ, &   System.double NewX, &   System.double NewY, &   System.double NewZ, &   System.bool LastMove ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OldX*
:   x coordinate of vertex to move

*OldY*
:   y coordinate of vertex to move

*OldZ*
:   z coordinate of vertex to move

*NewX*
:   x coordinate where to move the vertex

*NewY*
:   y coordinate where to move the vertex

*NewZ*
:   z coordinate where to move the vertex

*LastMove*
:   True if this move is the last move in a series of moves to close the gap, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::ImportDiagnosisGapCloser.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::ImportDiagnosis Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ImportDiagnosis.html)

[IBody2::Diagnose Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Diagnose.html)

[IDiagnoseResult Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDiagnoseResult.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0