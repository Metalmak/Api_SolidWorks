<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D~Get3DViewAnnotationTextScale.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Get3DViewAnnotationTextScale Method (IView3D) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView3D Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html) : Get3DViewAnnotationTextScale Method (IView3D) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Scale1*
:   Numerator of the scale ratio (**n**:n)

*Scale2*
:   Denominator of the scale ratio (n:**n**)

Gets the annotation text scale for this 3D View.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Get3DViewAnnotationTextScale( _    ByRef Scale1 As System.Double, _    ByRef Scale2 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView3D Dim Scale1 As System.Double Dim Scale2 As System.Double   instance.Get3DViewAnnotationTextScale(Scale1, Scale2) ``` | |

| C# |  |
| --- | --- |
| ``` void Get3DViewAnnotationTextScale(     out System.double Scale1,    out System.double Scale2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Get3DViewAnnotationTextScale(  &   [Out] System.double Scale1, &   [Out] System.double Scale2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Scale1*
:   Numerator of the scale ratio (**n**:n)

*Scale2*
:   Denominator of the scale ratio (n:**n**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View3D::Get3DViewAnnotationTextScale.

# ![](dotnetimages/collapse.gif)Remarks

This method gets the **Text scale** on the Annotation Properties dialog that appears when you RMB on the Annotations folder in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif)See Also

####

[IView3D Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D.html)

[IView3D Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView3D_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0