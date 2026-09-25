<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet~Select.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Select Method (IFacet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFacet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html) : Select Method (IFacet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Append*
:   True to append this selection to the selection list, false to replace the selection list with this selection

*Data*
:   Pointer to the [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) object

Selects the specified facet.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Select( _    ByVal Append As System.Boolean, _    ByVal Data As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFacet Dim Append As System.Boolean Dim Data As System.Object Dim value As System.Boolean   value = instance.Select(Append, Data) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Select(     System.bool Append,    System.object Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Select(  &   System.bool Append, &   System.Object^ Data ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Append*
:   True to append this selection to the selection list, false to replace the selection list with this selection

*Data*
:   Pointer to the [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) object

#### Return Value

True if the facet is selected, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Facet::Select.

# ![](dotnetimages/collapse.gif)Example

See the [IFacet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IFacet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet.html)

[IFacet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFacet_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30