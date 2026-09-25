<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AddToolbar2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddToolbar2 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AddToolbar2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModuleNameIn*

*TitleIn*

*SmallBitmapHandleIn*

*LargeBitmapHandleIn*

*MenuPosIn*

*DecTemplateTypeIn*

Obsolete. Superseded by [ISldWorks::AddToolbar4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~AddToolbar4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddToolbar2( _    ByVal ModuleNameIn As System.String, _    ByVal TitleIn As System.String, _    ByVal SmallBitmapHandleIn As System.Integer, _    ByVal LargeBitmapHandleIn As System.Integer, _    ByVal MenuPosIn As System.Integer, _    ByVal DecTemplateTypeIn As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ModuleNameIn As System.String Dim TitleIn As System.String Dim SmallBitmapHandleIn As System.Integer Dim LargeBitmapHandleIn As System.Integer Dim MenuPosIn As System.Integer Dim DecTemplateTypeIn As System.Integer Dim value As System.Integer   value = instance.AddToolbar2(ModuleNameIn, TitleIn, SmallBitmapHandleIn, LargeBitmapHandleIn, MenuPosIn, DecTemplateTypeIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddToolbar2(     System.string ModuleNameIn,    System.string TitleIn,    System.int SmallBitmapHandleIn,    System.int LargeBitmapHandleIn,    System.int MenuPosIn,    System.int DecTemplateTypeIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddToolbar2(  &   System.String^ ModuleNameIn, &   System.String^ TitleIn, &   System.int SmallBitmapHandleIn, &   System.int LargeBitmapHandleIn, &   System.int MenuPosIn, &   System.int DecTemplateTypeIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModuleNameIn*

*TitleIn*

*SmallBitmapHandleIn*

*LargeBitmapHandleIn*

*MenuPosIn*

*DecTemplateTypeIn*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AddToolbar2.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)