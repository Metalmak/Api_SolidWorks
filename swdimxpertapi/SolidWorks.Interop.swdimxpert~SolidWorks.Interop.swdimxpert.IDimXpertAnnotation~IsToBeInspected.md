<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation~IsToBeInspected.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| IsToBeInspected Method (IDimXpertAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertAnnotation Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation.html) : IsToBeInspected Method (IDimXpertAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether this annotation is to be inspected.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsToBeInspected() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertAnnotation Dim value As System.Boolean   value = instance.IsToBeInspected() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsToBeInspected() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsToBeInspected(); ``` | |

#### Return Value

True if to be inspected; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertAnnotation::IsToBeInspected.

# ![](dotnetimages/collapse.gif)Remarks

This tolerance modifier is set by clicking the second option from the right on the Dimension Text section of the DimXpert Properties manager.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertAnnotation Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation.html)

[IDimXpertAnnotation Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0