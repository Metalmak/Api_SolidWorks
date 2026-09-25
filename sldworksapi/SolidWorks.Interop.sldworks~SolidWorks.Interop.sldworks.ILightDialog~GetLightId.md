<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog~GetLightId.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetLightId Method (ILightDialog) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILightDialog Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog.html) : GetLightId Method (ILightDialog) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the ID of the edited light in the light dialog.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetLightId() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILightDialog Dim value As System.Integer   value = instance.GetLightId() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLightId() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLightId(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

ID of the light currently being modified by the dialog; -1 if the light cannot be found

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LightDialog::GetLightId.

# ![](dotnetimages/collapse.gif)See Also

####

[ILightDialog Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog.html)

[ILightDialog Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILightDialog_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, Revision Number 1999207