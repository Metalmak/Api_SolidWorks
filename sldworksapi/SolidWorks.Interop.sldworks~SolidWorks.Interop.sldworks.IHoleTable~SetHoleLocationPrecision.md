<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~SetHoleLocationPrecision.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetHoleLocationPrecision Method (IHoleTable) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html) : SetHoleLocationPrecision Method (IHoleTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseDoc*
:   True to set the location for this hole table using the document's precision, false
    to not

*Precision*
:   Precision to use for location values if UseDoc set to false

Sets the precision to use for location values for this hole table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetHoleLocationPrecision( _    ByVal UseDoc As System.Boolean, _    ByVal Precision As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleTable Dim UseDoc As System.Boolean Dim Precision As System.Integer Dim value As System.Boolean   value = instance.SetHoleLocationPrecision(UseDoc, Precision) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetHoleLocationPrecision(     System.bool UseDoc,    System.int Precision ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetHoleLocationPrecision(  &   System.bool UseDoc, &   System.int Precision ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseDoc*
:   True to set the location for this hole table using the document's precision, false
    to not

*Precision*
:   Precision to use for location values if UseDoc set to false

#### Return Value

True if precision is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleTable::SetHoleLocationPrecision.

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html)

[IHoleTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable_members.html)

[IHoleTable::GetHoleLocationPrecision Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetHoleLocationPrecision.html)

[IHoleTable::GetHoleLocationUseDocPrecision Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetHoleLocationUseDocPrecision.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0