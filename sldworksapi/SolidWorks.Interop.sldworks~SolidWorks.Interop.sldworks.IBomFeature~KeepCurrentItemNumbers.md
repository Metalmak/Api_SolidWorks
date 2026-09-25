<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature~KeepCurrentItemNumbers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| KeepCurrentItemNumbers Property (IBomFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html) : KeepCurrentItemNumbers Property (IBomFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether item numbers are kept with their components when reordering rows of a BOM table.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property KeepCurrentItemNumbers As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomFeature Dim value As System.Boolean   instance.KeepCurrentItemNumbers = value   value = instance.KeepCurrentItemNumbers ``` | |

| C# |  |
| --- | --- |
| ``` System.bool KeepCurrentItemNumbers {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool KeepCurrentItemNumbers {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if item numbers are kept with their components when reordering rows, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BomFeature::KeepCurrentItemNumbers.

# ![](dotnetimages/collapse.gif)Example

See [IBomFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Rows in a BOM table can be reordered in several different ways. For example, you can interactively reorder the rows manually in the Bill of Materials Properties dialog box and you can programmatically reorder rows using [IBomFeature::FollowAssemblyOrder2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomFeature~FollowAssemblyOrder2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IBomFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature.html)

[IBomFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12