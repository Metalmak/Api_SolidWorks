<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote~GetBendLineValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBendLineValues2 Method (INote) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html) : GetBendLineValues2 Method (INote) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Up*
:   True if the bend is up, false if the bend is down

*Angle*
:   Angle of the bend

*Radius*
:   Radius of the bend

*Points*
:   Array of doubles (see Remarks)

Gets the values of a bend line note.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBendLineValues2( _    ByRef Up As System.Boolean, _    ByRef Angle As System.Double, _    ByRef Radius As System.Double, _    ByRef Points As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As INote Dim Up As System.Boolean Dim Angle As System.Double Dim Radius As System.Double Dim Points As System.Object Dim value As System.Boolean   value = instance.GetBendLineValues2(Up, Angle, Radius, Points) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetBendLineValues2(     out System.bool Up,    out System.double Angle,    out System.double Radius,    out System.object Points ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetBendLineValues2(  &   [Out] System.bool Up, &   [Out] System.double Angle, &   [Out] System.double Radius, &   [Out] System.Object^ Points ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Up*
:   True if the bend is up, false if the bend is down

*Angle*
:   Angle of the bend

*Radius*
:   Radius of the bend

*Points*
:   Array of doubles (see Remarks)

#### Return Value

True if the note is a bend note, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Note::GetBendLineValues2.

# ![](dotnetimages/collapse.gif)Remarks

Points will contain six (6) doubles (three (3) each for the start point and endpoint), one set for each segment in the bend line:

[  x, y, z, x, y, z ]

# ![](dotnetimages/collapse.gif)See Also

####

[INote Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)

[INote Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote_members.html)

[IMathPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMathPoint.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0