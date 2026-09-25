<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFolder~GetSheetMetals.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSheetMetals Method (ISheetMetalFolder) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheetMetalFolder Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFolder.html) : GetSheetMetals Method (ISheetMetalFolder) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the sheet metal features in this folder.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSheetMetals() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheetMetalFolder Dim value As System.Object   value = instance.GetSheetMetals() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSheetMetals() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSheetMetals(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)s

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SheetMetalFolder::GetSheetMetals.

# ![](dotnetimages/collapse.gif)Example

See [ISheetMetalFolder](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISheetMetalFolder.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheetMetalFolder Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFolder.html)

[ISheetMetalFolder Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFolder_members.html)

[ISheetMetalFolder::GetSheetMetalCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheetMetalFolder~GetSheetMetalCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0