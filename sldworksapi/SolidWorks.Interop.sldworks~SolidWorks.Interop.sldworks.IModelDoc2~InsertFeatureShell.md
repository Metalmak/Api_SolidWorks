<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertFeatureShell.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertFeatureShell Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertFeatureShell Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Thickness*
:   Shell thickness in meters

*Outward*
:   True for outside, false for inside

Creates a shell feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertFeatureShell( _    ByVal Thickness As System.Double, _    ByVal Outward As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Thickness As System.Double Dim Outward As System.Boolean   instance.InsertFeatureShell(Thickness, Outward) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertFeatureShell(     System.double Thickness,    System.bool Outward ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertFeatureShell(  &   System.double Thickness, &   System.bool Outward ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Thickness*
:   Shell thickness in meters

*Outward*
:   True for outside, false for inside

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertFeatureShell.

# ![](dotnetimages/collapse.gif)Example

[Create Shell Feature (VBA)](Get_Shell_Feature_Data_Example_VB.htm)

[Create Shell Feature (VB.NET)](Create_Shell_Feature_Example_VBNET.htm)

[Create Shell Feature (C#)](Create_Shell_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select faces to remove to create the shell using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Marks of 1. See the SOLIDWORKS Help for information about what entities are valid for selection.

To make a multi-thickness shell, use this method with [IModelDoc2::InsertFeatureShellAddThickness](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertFeatureShellAddThickness.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IShellFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IShellFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0