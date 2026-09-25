<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddToolbar3 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddToolbar3 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Cookie*

*Title*

*SmallBitmapResourceID*

*LargeBitmapResourceID*

*MenuPositionForToolbar*

*DocumentType*

Obsolete. Superseded by [ISldWorks::AddToolbar4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~AddToolbar4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddToolbar3( _    ByVal Cookie As System.Integer, _    ByVal Title As System.String, _    ByVal SmallBitmapResourceID As System.Integer, _    ByVal LargeBitmapResourceID As System.Integer, _    ByVal MenuPositionForToolbar As System.Integer, _    ByVal DocumentType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Cookie As System.Integer Dim Title As System.String Dim SmallBitmapResourceID As System.Integer Dim LargeBitmapResourceID As System.Integer Dim MenuPositionForToolbar As System.Integer Dim DocumentType As System.Integer Dim value As System.Integer   value = instance.AddToolbar3(Cookie, Title, SmallBitmapResourceID, LargeBitmapResourceID, MenuPositionForToolbar, DocumentType) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddToolbar3(     System.int Cookie,    System.string Title,    System.int SmallBitmapResourceID,    System.int LargeBitmapResourceID,    System.int MenuPositionForToolbar,    System.int DocumentType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddToolbar3(  &   System.int Cookie, &   System.String^ Title, &   System.int SmallBitmapResourceID, &   System.int LargeBitmapResourceID, &   System.int MenuPositionForToolbar, &   System.int DocumentType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Cookie*

*Title*

*SmallBitmapResourceID*

*LargeBitmapResourceID*

*MenuPositionForToolbar*

*DocumentType*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddToolbar3.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)