<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~ICreateSectionViewAt3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateSectionViewAt3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : ICreateSectionViewAt3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*

*Y*

*Z*

*NotAligned*

*IsOffsetSection*

*Label*

*Chgdirection*

*Scwithmodel*

*Partial*

*Dispsurfcut*

*NumExcludedComponents*

*PExcludedComponents*

Obsolete. Superseded by [IDrawingDoc::ICreateSectionViewAt4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~CreateSectionViewAt4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateSectionViewAt3( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal NotAligned As System.Boolean, _    ByVal IsOffsetSection As System.Boolean, _    ByVal Label As System.String, _    ByVal Chgdirection As System.Boolean, _    ByVal Scwithmodel As System.Boolean, _    ByVal Partial As System.Boolean, _    ByVal Dispsurfcut As System.Boolean, _    ByVal NumExcludedComponents As System.Integer, _    ByRef PExcludedComponents As System.Object _ ) As View ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim NotAligned As System.Boolean Dim IsOffsetSection As System.Boolean Dim Label As System.String Dim Chgdirection As System.Boolean Dim Scwithmodel As System.Boolean Dim Partial As System.Boolean Dim Dispsurfcut As System.Boolean Dim NumExcludedComponents As System.Integer Dim PExcludedComponents As System.Object Dim value As View   value = instance.ICreateSectionViewAt3(X, Y, Z, NotAligned, IsOffsetSection, Label, Chgdirection, Scwithmodel, Partial, Dispsurfcut, NumExcludedComponents, PExcludedComponents) ``` | |

| C# |  |
| --- | --- |
| ``` View ICreateSectionViewAt3(     System.double X,    System.double Y,    System.double Z,    System.bool NotAligned,    System.bool IsOffsetSection,    System.string Label,    System.bool Chgdirection,    System.bool Scwithmodel,    System.bool Partial,    System.bool Dispsurfcut,    System.int NumExcludedComponents,    ref System.object PExcludedComponents ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` View^ ICreateSectionViewAt3(  &   System.double X, &   System.double Y, &   System.double Z, &   System.bool NotAligned, &   System.bool IsOffsetSection, &   System.String^ Label, &   System.bool Chgdirection, &   System.bool Scwithmodel, &   System.bool Partial, &   System.bool Dispsurfcut, &   System.int NumExcludedComponents, &   System.Object^% PExcludedComponents ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*

*Y*

*Z*

*NotAligned*

*IsOffsetSection*

*Label*

*Chgdirection*

*Scwithmodel*

*Partial*

*Dispsurfcut*

*NumExcludedComponents*

*PExcludedComponents*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::ICreateSectionViewAt3.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)