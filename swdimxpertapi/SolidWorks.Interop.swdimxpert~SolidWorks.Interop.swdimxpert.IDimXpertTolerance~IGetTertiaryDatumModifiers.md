<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertTolerance~IGetTertiaryDatumModifiers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| IGetTertiaryDatumModifiers Method (IDimXpertTolerance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertTolerance Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertTolerance.html) : IGetTertiaryDatumModifiers Method (IDimXpertTolerance) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of tertiary datum modifiers

Gets all of the tertiary datum modifiers in this DimXpert geometric tolerance annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetTertiaryDatumModifiers( _    ByVal Count As System.Integer _ ) As swDimXpertMaterialConditionModifier_e ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertTolerance Dim Count As System.Integer Dim value As swDimXpertMaterialConditionModifier_e   value = instance.IGetTertiaryDatumModifiers(Count) ``` | |

| C# |  |
| --- | --- |
| ``` swDimXpertMaterialConditionModifier_e IGetTertiaryDatumModifiers(     System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` swDimXpertMaterialConditionModifier_e IGetTertiaryDatumModifiers(  &   System.int Count ) ``` | |

#### Parameters

*Count*
:   Number of tertiary datum modifiers

#### Return Value

- in-process, unmanaged C++: Pointer to an array of integers- VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

See In-process Methods for details about this type of method.

Before calling this method, call [IDimXpertTolerance::GetTertiaryDatumCount](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertTolerance~GetTertiaryDatumCount.html) to get the value for the Count parameter.

The members of the array returned by this method map to the members of the array returned by [IGetDimXpertTolerance::IGetTertiaryDatums](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertTolerance~IGetTertiaryDatums.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertTolerance Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertTolerance.html)

[IDimXpertTolerance Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertTolerance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0