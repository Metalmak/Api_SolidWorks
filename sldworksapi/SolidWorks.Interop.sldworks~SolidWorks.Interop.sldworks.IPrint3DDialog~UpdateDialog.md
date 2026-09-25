<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrint3DDialog~UpdateDialog.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UpdateDialog Method (IPrint3DDialog) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPrint3DDialog Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrint3DDialog.html) : UpdateDialog Method (IPrint3DDialog) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Updates the build statistics on the Print 3D dialog for a local 3D printer.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function UpdateDialog() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPrint3DDialog Dim value As System.Boolean   value = instance.UpdateDialog() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UpdateDialog() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool UpdateDialog(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if the statistics are updated, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Print3DDialog::UpdateDialog.

# ![](dotnetimages/collapse.gif)See Also

####

[IPrint3DDialog Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrint3DDialog.html)

[IPrint3DDialog Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPrint3DDialog_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP1, Revision Number 15.1