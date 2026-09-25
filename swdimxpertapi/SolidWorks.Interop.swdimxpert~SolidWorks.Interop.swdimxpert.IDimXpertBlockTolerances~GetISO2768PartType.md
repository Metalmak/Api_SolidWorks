<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertBlockTolerances~GetISO2768PartType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetISO2768PartType Method (IDimXpertBlockTolerances) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertBlockTolerances Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertBlockTolerances.html) : GetISO2768PartType Method (IDimXpertBlockTolerances) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   ISO 2768 part type of this DimXpert block tolerance as defined in [swDimXpertISO2768PartType\_e](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertISO2768PartType_e.html)

Gets the ISO 2768 part type of this DimXpert block tolerance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetISO2768PartType( _    ByRef Type As swDimXpertISO2768PartType_e _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertBlockTolerances Dim Type As swDimXpertISO2768PartType_e Dim value As System.Boolean   value = instance.GetISO2768PartType(Type) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetISO2768PartType(     out swDimXpertISO2768PartType_e Type ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetISO2768PartType(  &   [Out] swDimXpertISO2768PartType_e Type ) ``` | |

#### Parameters

*Type*
:   ISO 2768 part type of this DimXpert block tolerance as defined in [swDimXpertISO2768PartType\_e](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertISO2768PartType_e.html)

#### Return Value

True if the method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertBlockTolerances::GetISO2768PartType.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpert Block Tolerance Example (VBA)](Get_DimXpert_Block_Tolerance_Example_VB.htm)

[Get DimXpert Block Tolerance Example (VB.NET)](Get_DimXpert_Block_Tolerance_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertBlockTolerances Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertBlockTolerances.html)

[IDimXpertBlockTolerances Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertBlockTolerances_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0