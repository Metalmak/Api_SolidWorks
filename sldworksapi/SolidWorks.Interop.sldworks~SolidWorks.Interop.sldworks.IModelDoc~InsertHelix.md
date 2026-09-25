<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertHelix.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertHelix Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertHelix Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Reversed*

*Clockwised*

*Tapered*

*Outward*

*Helixdef*

*Height*

*Pitch*

*Revolution*

*TaperAngle*

*Startangle*

Obsolete. Superseded by [IModelDoc2::InsertHelix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertHelix.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertHelix( _    ByVal Reversed As System.Boolean, _    ByVal Clockwised As System.Boolean, _    ByVal Tapered As System.Boolean, _    ByVal Outward As System.Boolean, _    ByVal Helixdef As System.Integer, _    ByVal Height As System.Double, _    ByVal Pitch As System.Double, _    ByVal Revolution As System.Double, _    ByVal TaperAngle As System.Double, _    ByVal Startangle As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Reversed As System.Boolean Dim Clockwised As System.Boolean Dim Tapered As System.Boolean Dim Outward As System.Boolean Dim Helixdef As System.Integer Dim Height As System.Double Dim Pitch As System.Double Dim Revolution As System.Double Dim TaperAngle As System.Double Dim Startangle As System.Double   instance.InsertHelix(Reversed, Clockwised, Tapered, Outward, Helixdef, Height, Pitch, Revolution, TaperAngle, Startangle) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertHelix(     System.bool Reversed,    System.bool Clockwised,    System.bool Tapered,    System.bool Outward,    System.int Helixdef,    System.double Height,    System.double Pitch,    System.double Revolution,    System.double TaperAngle,    System.double Startangle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertHelix(  &   System.bool Reversed, &   System.bool Clockwised, &   System.bool Tapered, &   System.bool Outward, &   System.int Helixdef, &   System.double Height, &   System.double Pitch, &   System.double Revolution, &   System.double TaperAngle, &   System.double Startangle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Reversed*

*Clockwised*

*Tapered*

*Outward*

*Helixdef*

*Height*

*Pitch*

*Revolution*

*TaperAngle*

*Startangle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertHelix.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)