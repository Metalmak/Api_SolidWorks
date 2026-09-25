<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart~InsertGtol.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| InsertGtol Method (IDimXpertPart) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html) : InsertGtol Method (IDimXpertPart) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of Gtol to insert as defined in [swDimXpertGtolType\_e](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.swDimXpertGtolType_e.html)

Inserts the specified Gtol annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertGtol( _    ByVal Type As System.Integer _ ) As DimXpertAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertPart Dim Type As System.Integer Dim value As DimXpertAnnotation   value = instance.InsertGtol(Type) ``` | |

| C# |  |
| --- | --- |
| ``` DimXpertAnnotation InsertGtol(     System.int Type ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DimXpertAnnotation^ InsertGtol(  &   System.int Type ) ``` | |

#### Parameters

*Type*
:   Type of Gtol to insert as defined in [swDimXpertGtolType\_e](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.swDimXpertGtolType_e.html)

#### Return Value

[IDimXpertAnnotation](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertPart::InsertGtol.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select the leader attachment points.

This method creates an empty Gtol symbol with a default value of 0.02 for Tolerance 1. To fill in the text and symbols, get the underlying SOLIDWORKS Gtol object and use IGtol::SetFrameSymbols2 and IGtol::SetFrameValues2 to change frame symbols and values.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertPart Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart.html)

[IDimXpertPart Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPart_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0