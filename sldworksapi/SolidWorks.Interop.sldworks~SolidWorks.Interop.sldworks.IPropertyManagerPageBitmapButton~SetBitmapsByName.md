<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton~SetBitmapsByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBitmapsByName Method (IPropertyManagerPageBitmapButton) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageBitmapButton Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton.html) : SetBitmapsByName Method (IPropertyManagerPageBitmapButton) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BitmapUp*

*BitmapDown*

*BitmapDisabled*

Obsolete. Superseded by [IPropertyManagerPageBitmapButton::SetBitmapsByName2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageBitmapButton~SetBitmapsByName2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBitmapsByName( _    ByVal BitmapUp As System.String, _    ByVal BitmapDown As System.String, _    ByVal BitmapDisabled As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageBitmapButton Dim BitmapUp As System.String Dim BitmapDown As System.String Dim BitmapDisabled As System.String Dim value As System.Boolean   value = instance.SetBitmapsByName(BitmapUp, BitmapDown, BitmapDisabled) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetBitmapsByName(     System.string BitmapUp,    System.string BitmapDown,    System.string BitmapDisabled ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetBitmapsByName(  &   System.String^ BitmapUp, &   System.String^ BitmapDown, &   System.String^ BitmapDisabled ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BitmapUp*

*BitmapDown*

*BitmapDisabled*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageBitmapButton::SetBitmapsByName.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageBitmapButton Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton.html)

[IPropertyManagerPageBitmapButton Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmapButton_members.html)