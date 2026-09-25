<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddComment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddComment Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : AddComment Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Text*
:   Comment to add to the document's Comment folder

Adds a comment to this document's Comment Folder.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddComment( _    ByVal Text As System.String _ ) As Comment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Text As System.String Dim value As Comment   value = instance.AddComment(Text) ``` | |

| C# |  |
| --- | --- |
| ``` Comment AddComment(     System.string Text ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Comment^ AddComment(  &   System.String^ Text ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Text*
:   Comment to add to the document's Comment folder

#### Return Value

[Comment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComment.html) folder

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::AddComment.

# ![](dotnetimages/collapse.gif)Example

[Add Comment to Assembly Component (VBA)](Add_Comment_to_Assembly_Component_Example_VB.htm)

[Add Comment to Assembly Component (VB.NET)](Add_Comment_to_Assembly_Component_Example_VBNET.htm)

[Add Comment to Assembly Component (C#)](Add_Comment_to_Assembly_Component_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A comment is added to the document's Comment folder, and the comment is associated with the preselected item when this method is run.

For example:

|  |  |
| --- | --- |
| **If...** | **Then the comment is...** |
| A feature is preselected | Associated with the feature (equivalent to running the [IFeature::AddComment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~AddComment.html) on the selected feature) |
| The Comment folder is preselected | Not associated with any feature, but is added to the Comment folder (equivalent to running the [ICommentFolder::AddComment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommentFolder~AddComment.html) method) |

Although it might appear that ModelDocExtension::AddComment duplicates IFeature::AddComment and ICommentFolder::AddComment, IModelDocExtension::AddComment is used when recording macros, so it is different. IModelDocExtension::AddComment shares code with the user interface, so it should behave identical to the user interface.

IModelDocExtension::AddComment rebuilds the FeatureManager design tree automatically, which can be a time-consuming operation if the FeatureManager design tree gets large. Take this into consideration before using it.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IComment::Delete Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComment~Delete.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0