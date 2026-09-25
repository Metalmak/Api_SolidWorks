<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComment~FeatureOwner.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureOwner Property (IComment) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComment.html) : FeatureOwner Property (IComment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the feature that owns this comment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property FeatureOwner As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComment Dim value As Feature   value = instance.FeatureOwner ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureOwner {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property Feature^ FeatureOwner {    Feature^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object that owns this comment

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Comment::FeatureOwner.

# ![](dotnetimages/collapse.gif)Remarks

If the comment is not owned by a feature, then NULL is returned.

Because you cannot set the name of comment owned by a feature, use this property before using [IComment::Name](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComment~Name.html) to determine if the comment is owned by a feature.

# ![](dotnetimages/collapse.gif)See Also

####

[IComment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComment.html)

[IComment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComment_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14