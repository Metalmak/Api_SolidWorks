<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ICreateFeatureFromBody4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICreateFeatureFromBody4 Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : ICreateFeatureFromBody4 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Body*
:   Temporary [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*MakeRefSurface*
:   If the body cannot be knit to a solid or if a solid body already exists in this model, then True creates of a reference surface feature

*Options*
:   Option as defined by swCreateFeatureBodyOpts\_e

Creates a new imported feature from the specified temporary body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ICreateFeatureFromBody4( _    ByVal Body As Body2, _    ByVal MakeRefSurface As System.Boolean, _    ByVal Options As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Body As Body2 Dim MakeRefSurface As System.Boolean Dim Options As System.Integer Dim value As Feature   value = instance.ICreateFeatureFromBody4(Body, MakeRefSurface, Options) ``` | |

| C# |  |
| --- | --- |
| ``` Feature ICreateFeatureFromBody4(     Body2 Body,    System.bool MakeRefSurface,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ ICreateFeatureFromBody4(  &   Body2^ Body, &   System.bool MakeRefSurface, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Body*
:   Temporary [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*MakeRefSurface*
:   If the body cannot be knit to a solid or if a solid body already exists in this model, then True creates of a reference surface feature

*Options*
:   Option as defined by swCreateFeatureBodyOpts\_e

#### Return Value

Newly created imported [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) or NULL if the operation fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::ICreateFeatureFromBody4.

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Is intended as the final call in a knitting operation. The body that results from your knitting efforts can be converted into an imported body feature in the SOLIDWORKS model.

  * Is not limited to [IBody2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) objects obtained from knitting operations.

    * Allows the application to decide how much additional work must be done to the model before creating the feature. The options listed in the swCreateFeatureBodyOpts\_e enumeration can be OR'd together to provide additional checking or simplification of the model. If you specify swCreateFeatureBodySimplify for Options, then swCreateFeatureBodyCheck is implied.

If the application passes 0 for the options argument, then the options are disabled and the model is passed without any checking. It is up to the application to ensure that the model is a valid model.

If this method fails, the error might be caused by creating a sheet (surface) body from a multiple shells body. If so, replace this method with [IPartDoc::CreateSurfaceFeatureFromBody](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc~CreateSurfaceFeatureFromBody.html) and [IPartDoc::ICreateSurfaceFeatureFromBodyCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc~ICreateSurfaceFeatureFromBodyCount2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::CreateFeatureFromBody3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~CreateFeatureFromBody3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0