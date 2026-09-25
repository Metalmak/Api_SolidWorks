<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetSecondArrow.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSecondArrow Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetSecondArrow Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseDoc*
:   True uses the document setting for second arrows, false uses the setting specified by the SecondArrow argument

*SecondArrow*
:   Enables or disables the display of the second arrow on this display dimension if UseDoc is false

Sets the second arrow characteristics of this diameter display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSecondArrow( _    ByVal UseDoc As System.Boolean, _    ByVal SecondArrow As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim UseDoc As System.Boolean Dim SecondArrow As System.Boolean   instance.SetSecondArrow(UseDoc, SecondArrow) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSecondArrow(     System.bool UseDoc,    System.bool SecondArrow ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSecondArrow(  &   System.bool UseDoc, &   System.bool SecondArrow ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseDoc*
:   True uses the document setting for second arrows, false uses the setting specified by the SecondArrow argument

*SecondArrow*
:   Enables or disables the display of the second arrow on this display dimension if UseDoc is false

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetSecondArrow.

# ![](dotnetimages/collapse.gif)Remarks

For diameter dimensions, the second outside arrow is the arrow that appears on the opposite side of the arc from the dimension text. This occurs only when the text is outside of the arc.

Display of this arrow is optional, and is controlled by a value stored in one of two places: on the owning document or on the individual display dimension. This method allows you to determine which setting to use: the document default or the value specified in the secondArrow argument.

The UseDoc argument indicates whether to use the document default setting for second arrows. If it is false, then the SecondArrow argument indicates whether or not the second arrow is enabled.

Use [IDisplayDimension::GetUseDocSecondArrow](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetUseDocSecondArrow.html) and [IDisplayDimension::GetSecondArrow](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetSecondArrow.html) to get the current values for these settings.

This method applies to only diameter dimensions. If you execute this method with any other types of dimensions, SOLIDWORKS returns false.

After using this method, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window to see your changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::ArrowSide Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~ArrowSide.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207