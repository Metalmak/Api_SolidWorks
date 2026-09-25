<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditBalloonProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditBalloonProperties Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : EditBalloonProperties Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*

*Size*

*UpperTextStyle*

*UpperText*

*LowerTextStyle*

*LowerText*

Obsolete. Superseded by [INote::SetBalloon](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~SetBalloon.html) and [INote::SetBomBalloonText](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote~SetBomBalloonText.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditBalloonProperties( _    ByVal Style As System.Integer, _    ByVal Size As System.Integer, _    ByVal UpperTextStyle As System.Integer, _    ByVal UpperText As System.String, _    ByVal LowerTextStyle As System.Integer, _    ByVal LowerText As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Style As System.Integer Dim Size As System.Integer Dim UpperTextStyle As System.Integer Dim UpperText As System.String Dim LowerTextStyle As System.Integer Dim LowerText As System.String Dim value As System.Object   value = instance.EditBalloonProperties(Style, Size, UpperTextStyle, UpperText, LowerTextStyle, LowerText) ``` | |

| C# |  |
| --- | --- |
| ``` System.object EditBalloonProperties(     System.int Style,    System.int Size,    System.int UpperTextStyle,    System.string UpperText,    System.int LowerTextStyle,    System.string LowerText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ EditBalloonProperties(  &   System.int Style, &   System.int Size, &   System.int UpperTextStyle, &   System.String^ UpperText, &   System.int LowerTextStyle, &   System.String^ LowerText ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*

*Size*

*UpperTextStyle*

*UpperText*

*LowerTextStyle*

*LowerText*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::EditBalloonProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)