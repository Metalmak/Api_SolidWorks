<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~AllowFailedFeatureCreation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AllowFailedFeatureCreation Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : AllowFailedFeatureCreation Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*YesNo*
:   True if features are to be created regardless of rebuild errors, false if not

Sets whether to allow the creation of a feature that has rebuild errors.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AllowFailedFeatureCreation( _    ByVal YesNo As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim YesNo As System.Boolean Dim value As System.Boolean   value = instance.AllowFailedFeatureCreation(YesNo) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AllowFailedFeatureCreation(     System.bool YesNo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AllowFailedFeatureCreation(  &   System.bool YesNo ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*YesNo*
:   True if features are to be created regardless of rebuild errors, false if not

#### Return Value

The previous value, which is now replaced by the value for YesNo

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::AllowFailedFeatureCreation.

# ![](dotnetimages/collapse.gif)Example

[Create Feature With Invalid Geometry (VBA)](Create_Feature_with_Invalid_Geometry_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

By default, features are not created when invalid geometry is specified; however, after calling this method with YesNo set to True, the features are created but with rebuild errors.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)