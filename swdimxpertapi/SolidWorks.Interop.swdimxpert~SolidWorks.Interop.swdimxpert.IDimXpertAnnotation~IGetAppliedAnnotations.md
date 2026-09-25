<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation~IGetAppliedAnnotations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| IGetAppliedAnnotations Method (IDimXpertAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertAnnotation Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation.html) : IGetAppliedAnnotations Method (IDimXpertAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of applied annotations

Gets all of the annotations applied to this DimXpert annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetAppliedAnnotations( _    ByVal Count As System.Integer _ ) As DimXpertAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertAnnotation Dim Count As System.Integer Dim value As DimXpertAnnotation   value = instance.IGetAppliedAnnotations(Count) ``` | |

| C# |  |
| --- | --- |
| ``` DimXpertAnnotation IGetAppliedAnnotations(     System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DimXpertAnnotation^ IGetAppliedAnnotations(  &   System.int Count ) ``` | |

#### Parameters

*Count*
:   Number of applied annotations

#### Return Value

- in-process, unmanaged C++: Pointer to an array of [IDimXpertAnnotation](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertAnnotation.html)- VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

See In-process Methods for details about this type of method.

Before calling this method, call [IDimXpertAnnotation::GetAppliedAnnotationCount](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertAnnotation~GetAppliedAnnotationCount.html) to get the value for the Count parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertAnnotation Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation.html)

[IDimXpertAnnotation Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0