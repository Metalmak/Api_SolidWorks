<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetLinkedText.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLinkedText Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetLinkedText Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BstrLinkedText*
:   Text to link to this display dimension

Sets the text to link to this display dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLinkedText( _    ByVal BstrLinkedText As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim BstrLinkedText As System.String Dim value As System.Integer   value = instance.SetLinkedText(BstrLinkedText) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetLinkedText(     System.string BstrLinkedText ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetLinkedText(  &   System.String^ BstrLinkedText ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BstrLinkedText*
:   Text to link to this display dimension

#### Return Value

Error code as defined in swLinkDimensionError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetLinkedText.

# ![](dotnetimages/collapse.gif)Remarks

* Dimension types must be the same, for example: linear to linea , angular to angular, and so on.

  * Angular dimensions must be in the same quadrant.

    * Dimensions cannot shared by another named group.

      * Dimensions with dissimilar ranges cannot be shared.

        * Dimensions cannot driven by equations, read-only, driven sketch dimensions, or reference dimensions.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::GetLinkedText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetLinkedText.html)

[IDisplayDimension::Unlink Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~Unlink.html)

[IDisplayDimension::IsLinked Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~IsLinked.html)