<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight~GetID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetID Method (ILight) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILight Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html) : GetID Method (ILight) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the light ID for this light feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetID() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILight Dim value As System.Integer   value = instance.GetID() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetID() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetID(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Light ID for this light feature

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Light::GetID.

# ![](dotnetimages/collapse.gif)Example

[Redirect Spotlight (VBA)](Redirect_Spotlight_Example_VB.htm)

[Add Spotlight and Get Light Feature (C#)](Add_Spotlight_and_Get_Light_Feature_Example_CSharp.htm)

[Add Spotlight and Get Light Feature (VB.NET)](Add_Spotlight_and_Get_Light_Feature_Example_VBNET.htm)

[Add Spotlight and Get Light Feature (VBA)](Add_Spotlight_and_Get_Light_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

A light ID:

* is unique within the document.* is persistent across SOLIDWORKS sessions and never changes, even if you change the name of the light.* can be used to identify a specific light in a document.* cannot be assigned by applications or users.* is not the same as a persistent reference ID. You can get a light using its persistent reference ID, but you cannot get a light using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ILight Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight.html)

[ILight Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILight_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0