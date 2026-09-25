<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature~Security.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| Security Method (ISwComFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwComFeature Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature.html) : Security Method (ISwComFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*app*
:   SOLIDWORKS application

*modelDoc*
:   SOLIDWORKS document in which the macro feature appears

*feature*
:   Macro feature whose security you want to set

Allows you to specify whether instances of the macro feature created using COM can be rolled back, edited, suppressed, replaced, or deleted from the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Security( _    ByVal app As System.Object, _    ByVal modelDoc As System.Object, _    ByVal feature As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwComFeature Dim app As System.Object Dim modelDoc As System.Object Dim feature As System.Object Dim value As System.Object   value = instance.Security(app, modelDoc, feature) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Security(     System.object app,    System.object modelDoc,    System.object feature ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Security(  &   System.Object^ app, &   System.Object^ modelDoc, &   System.Object^ feature ) ``` | |

#### Parameters

*app*
:   SOLIDWORKS application

*modelDoc*
:   SOLIDWORKS document in which the macro feature appears

*feature*
:   Macro feature whose security you want to set

#### Return Value

Value or combination of values as defined by swMacroFeatureSecurityOptions\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwComFeature::Security.

# ![](dotnetimages/collapse.gif)Remarks

This method also allows you to display a note associated with the macro feature to the end user. This method is required for COM-based macro features. See Overview of Macro Features for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwComFeature Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature.html)

[ISwComFeature Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0