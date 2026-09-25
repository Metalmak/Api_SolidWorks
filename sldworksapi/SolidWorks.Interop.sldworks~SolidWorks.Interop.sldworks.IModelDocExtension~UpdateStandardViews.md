<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateStandardViews.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UpdateStandardViews Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : UpdateStandardViews Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ViewName*
:   Name of the standard model view to change; empty string to use ViewId (**see Remarks**)

*ViewId*
:   View ID as defined in swStandardViews\_e; -1 to use ViewName (**see Remarks**)

Changes the specified standard view to the current model view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function UpdateStandardViews( _    ByVal ViewName As System.String, _    ByVal ViewId As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ViewName As System.String Dim ViewId As System.Integer Dim value As System.Boolean   value = instance.UpdateStandardViews(ViewName, ViewId) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UpdateStandardViews(     System.string ViewName,    System.int ViewId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool UpdateStandardViews(  &   System.String^ ViewName, &   System.int ViewId ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ViewName*
:   Name of the standard model view to change; empty string to use ViewId (**see Remarks**)

*ViewId*
:   View ID as defined in swStandardViews\_e; -1 to use ViewName (**see Remarks**)

#### Return Value

True if the standard model view update is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::UpdateStandardViews.

# ![](dotnetimages/collapse.gif)Remarks

This method works with parts and assemblies only.

If you set both ViewName and ViewId, then ViewId takes precedence if the two arguments do not resolve to the same standard model view.

This method does not support the following standard model views:

* swStandardViews\_e.swDimetricView* swStandardViews\_e.swIsometricView* swStandardViews\_e.swTrimetricView

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::ResetStandardViews Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ResetStandardViews.html)

[IModelDoc2::ShowNamedView2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ShowNamedView2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0