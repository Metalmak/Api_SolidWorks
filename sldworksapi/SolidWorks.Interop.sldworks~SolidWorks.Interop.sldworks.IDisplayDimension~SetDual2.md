<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetDual2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDual2 Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetDual2 Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseDoc*
:   True uses the document setting, false uses the opposite of the document setting (see **Remarks**)

*InwardRounding*
:   True for inward rounding of secondary unit tolerances, false for current document rounding (see **Remarks**)

Controls the display of dual dimensions of this display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetDual2( _    ByVal UseDoc As System.Boolean, _    ByVal InwardRounding As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim UseDoc As System.Boolean Dim InwardRounding As System.Boolean   instance.SetDual2(UseDoc, InwardRounding) ``` | |

| C# |  |
| --- | --- |
| ``` void SetDual2(     System.bool UseDoc,    System.bool InwardRounding ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetDual2(  &   System.bool UseDoc, &   System.bool InwardRounding ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseDoc*
:   True uses the document setting, false uses the opposite of the document setting (see **Remarks**)

*InwardRounding*
:   True for inward rounding of secondary unit tolerances, false for current document rounding (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetDual2.

# ![](dotnetimages/collapse.gif)Example

[Set Rounding of Decimal Units in Display Dimensions (VBA)](Set_Rounding_of_Decimal_Units_in_Display_Dimensions_Example_VB.htm)

[Set Rounding of Decimal Units in Display Dimensions (VB.NET)](Set_Rounding_of_Decimal_Units_in_Display_Dimensions_Example_VBNET.htm)

[Set Rounding of Decimal Units in Display Dimensions (C#)](Set_Rounding_of_Decimal_Units_in_Display_Dimensions_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Dual dimensions can use either the same top, bottom, right, or left setting as the document or an opposite top, bottom, right, or left setting. This method allows you to set a dual dimension to use the current document setting or the opposite setting.

| If InwardRounding is false and an override unit is... | Then... |
| --- | --- |
| Not specified | Current document rounding prevails |
| Specified | Rounding setting under **Override Units** in the Dimensions PropertyManager page prevails |

Use [IDisplayDimension::GetUseDocDual](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetUseDocDual.html) to get the current value of this setting.

After using this method, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window to see your changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::Split Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~Split.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0