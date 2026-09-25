<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddMenuPopupItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuPopupItem Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddMenuPopupItem Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DocType*

*SelType*

*Item*

*CallbackFcnAndModule*

*CustomNames*

Obsolete. Superseded by [ISldWorks::AddMenuPopupItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~AddMenuPopupItem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuPopupItem( _    ByVal DocType As System.Integer, _    ByVal SelType As System.Integer, _    ByVal Item As System.String, _    ByVal CallbackFcnAndModule As System.String, _    ByVal CustomNames As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim DocType As System.Integer Dim SelType As System.Integer Dim Item As System.String Dim CallbackFcnAndModule As System.String Dim CustomNames As System.String Dim value As System.Integer   value = instance.AddMenuPopupItem(DocType, SelType, Item, CallbackFcnAndModule, CustomNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddMenuPopupItem(     System.int DocType,    System.int SelType,    System.string Item,    System.string CallbackFcnAndModule,    System.string CustomNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddMenuPopupItem(  &   System.int DocType, &   System.int SelType, &   System.String^ Item, &   System.String^ CallbackFcnAndModule, &   System.String^ CustomNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DocType*

*SelType*

*Item*

*CallbackFcnAndModule*

*CustomNames*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddMenuPopupItem.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)