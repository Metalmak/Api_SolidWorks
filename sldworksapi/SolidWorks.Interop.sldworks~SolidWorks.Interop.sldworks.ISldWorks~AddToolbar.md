<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddToolbar Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddToolbar Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModuleName*

*Title*

*SmallBitmapHandle*

*LargeBitmapHandle*

Obsolete. Superseded by [ISldWorks::AddToolbar4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~AddToolbar4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddToolbar( _    ByVal ModuleName As System.String, _    ByVal Title As System.String, _    ByVal SmallBitmapHandle As System.Integer, _    ByVal LargeBitmapHandle As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ModuleName As System.String Dim Title As System.String Dim SmallBitmapHandle As System.Integer Dim LargeBitmapHandle As System.Integer Dim value As System.Integer   value = instance.AddToolbar(ModuleName, Title, SmallBitmapHandle, LargeBitmapHandle) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddToolbar(     System.string ModuleName,    System.string Title,    System.int SmallBitmapHandle,    System.int LargeBitmapHandle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddToolbar(  &   System.String^ ModuleName, &   System.String^ Title, &   System.int SmallBitmapHandle, &   System.int LargeBitmapHandle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModuleName*

*Title*

*SmallBitmapHandle*

*LargeBitmapHandle*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddToolbar.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)