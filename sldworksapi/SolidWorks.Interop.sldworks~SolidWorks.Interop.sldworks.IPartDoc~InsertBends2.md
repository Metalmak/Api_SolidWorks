<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertBends2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBends2 Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : InsertBends2 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Radius*
:   Radius of the bends

*UseBendTable*
:   Bend table name (.btl file)

*UseKfactor*
:   K-Factor ratio or -1 if not used

*UseBendAllowance*
:   Bend allowance value or -1 if not used

*UseAutoRelief*
:   True if auto-relief cuts are to be added, false if not

*OffsetRatio*
:   Distance relief cut extends beyond bend (see **Remarks)**

*DoFlatten*
:   True to create these three features: Sheet-Metal, Flatten-Bends, and Process-Bends, false to create only the Sheet-Metal feature

Creates bends in a thin-feature part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBends2( _    ByVal Radius As System.Double, _    ByVal UseBendTable As System.String, _    ByVal UseKfactor As System.Double, _    ByVal UseBendAllowance As System.Double, _    ByVal UseAutoRelief As System.Boolean, _    ByVal OffsetRatio As System.Double, _    ByVal DoFlatten As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Radius As System.Double Dim UseBendTable As System.String Dim UseKfactor As System.Double Dim UseBendAllowance As System.Double Dim UseAutoRelief As System.Boolean Dim OffsetRatio As System.Double Dim DoFlatten As System.Boolean Dim value As System.Boolean   value = instance.InsertBends2(Radius, UseBendTable, UseKfactor, UseBendAllowance, UseAutoRelief, OffsetRatio, DoFlatten) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertBends2(     System.double Radius,    System.string UseBendTable,    System.double UseKfactor,    System.double UseBendAllowance,    System.bool UseAutoRelief,    System.double OffsetRatio,    System.bool DoFlatten ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertBends2(  &   System.double Radius, &   System.String^ UseBendTable, &   System.double UseKfactor, &   System.double UseBendAllowance, &   System.bool UseAutoRelief, &   System.double OffsetRatio, &   System.bool DoFlatten ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Radius*
:   Radius of the bends

*UseBendTable*
:   Bend table name (.btl file)

*UseKfactor*
:   K-Factor ratio or -1 if not used

*UseBendAllowance*
:   Bend allowance value or -1 if not used

*UseAutoRelief*
:   True if auto-relief cuts are to be added, false if not

*OffsetRatio*
:   Distance relief cut extends beyond bend (see **Remarks)**

*DoFlatten*
:   True to create these three features: Sheet-Metal, Flatten-Bends, and Process-Bends, false to create only the Sheet-Metal feature

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::InsertBends2.

# ![](dotnetimages/collapse.gif)Remarks

The offsetRatio argument is from 0.05 to 2.0.  Any other value fails to create the
bend features.

When True is passed to doFlatten, all three Sheet-Metal features are created.

For more information on these arguments, see SOLIDWORKS Help.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0