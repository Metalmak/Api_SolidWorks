<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertBends.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBends Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : InsertBends Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Radius*

*UseBendTable*

*UseKfactor*

*UseBendAllowance*

*UseAutoRelief*

*OffsetRatio*

Obsolete. Superseded by [IPartDoc::InsertBends2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc~InsertBends2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBends( _    ByVal Radius As System.Double, _    ByVal UseBendTable As System.String, _    ByVal UseKfactor As System.Double, _    ByVal UseBendAllowance As System.Double, _    ByVal UseAutoRelief As System.Boolean, _    ByVal OffsetRatio As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Radius As System.Double Dim UseBendTable As System.String Dim UseKfactor As System.Double Dim UseBendAllowance As System.Double Dim UseAutoRelief As System.Boolean Dim OffsetRatio As System.Double Dim value As System.Boolean   value = instance.InsertBends(Radius, UseBendTable, UseKfactor, UseBendAllowance, UseAutoRelief, OffsetRatio) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertBends(     System.double Radius,    System.string UseBendTable,    System.double UseKfactor,    System.double UseBendAllowance,    System.bool UseAutoRelief,    System.double OffsetRatio ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertBends(  &   System.double Radius, &   System.String^ UseBendTable, &   System.double UseKfactor, &   System.double UseBendAllowance, &   System.bool UseAutoRelief, &   System.double OffsetRatio ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Radius*

*UseBendTable*

*UseKfactor*

*UseBendAllowance*

*UseAutoRelief*

*OffsetRatio*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::InsertBends.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)