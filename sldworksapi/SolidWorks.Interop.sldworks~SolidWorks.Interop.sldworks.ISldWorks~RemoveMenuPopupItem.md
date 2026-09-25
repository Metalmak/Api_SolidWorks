<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RemoveMenuPopupItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RemoveMenuPopupItem Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RemoveMenuPopupItem Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocType*

*SelectType*

*Item*

*CallbackFcnAndModule*

*CustomNames*

*Unused*

Obsolete. Superseded by [ISldWorks::RemoveMenuPopupItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RemoveMenuPopupItem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RemoveMenuPopupItem( _    ByVal DocType As System.Integer, _    ByVal SelectType As System.Integer, _    ByVal Item As System.String, _    ByVal CallbackFcnAndModule As System.String, _    ByVal CustomNames As System.String, _    ByVal Unused As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DocType As System.Integer Dim SelectType As System.Integer Dim Item As System.String Dim CallbackFcnAndModule As System.String Dim CustomNames As System.String Dim Unused As System.Integer Dim value As System.Boolean   value = instance.RemoveMenuPopupItem(DocType, SelectType, Item, CallbackFcnAndModule, CustomNames, Unused) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RemoveMenuPopupItem(     System.int DocType,    System.int SelectType,    System.string Item,    System.string CallbackFcnAndModule,    System.string CustomNames,    System.int Unused ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RemoveMenuPopupItem(  &   System.int DocType, &   System.int SelectType, &   System.String^ Item, &   System.String^ CallbackFcnAndModule, &   System.String^ CustomNames, &   System.int Unused ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocType*

*SelectType*

*Item*

*CallbackFcnAndModule*

*CustomNames*

*Unused*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RemoveMenuPopupItem.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)