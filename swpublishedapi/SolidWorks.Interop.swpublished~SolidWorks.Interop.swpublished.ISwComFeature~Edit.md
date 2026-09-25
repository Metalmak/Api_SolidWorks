<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature~Edit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| Edit Method (ISwComFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwComFeature Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature.html) : Edit Method (ISwComFeature) |

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
:   Macro feature whose definition you want to edit

Allows you to edit the definition of a macro feature created using COM.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Edit( _    ByVal app As System.Object, _    ByVal modelDoc As System.Object, _    ByVal feature As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwComFeature Dim app As System.Object Dim modelDoc As System.Object Dim feature As System.Object Dim value As System.Object   value = instance.Edit(app, modelDoc, feature) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Edit(     System.object app,    System.object modelDoc,    System.object feature ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Edit(  &   System.Object^ app, &   System.Object^ modelDoc, &   System.Object^ feature ) ``` | |

#### Parameters

*app*
:   SOLIDWORKS application

*modelDoc*
:   SOLIDWORKS document in which the macro feature appears

*feature*
:   Macro feature whose definition you want to edit

#### Return Value

True if editing the definition of the macro feature is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwComFeature::Edit.

# ![](dotnetimages/collapse.gif)Remarks

This method is required. See Exposed COM DLL or Executable and Macro Features and Overview of Macro Features for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwComFeature Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature.html)

[ISwComFeature Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwComFeature_members.html)

IFeatureManager::InsertSecurityNote Method

IMacroFeatureData Interface

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0