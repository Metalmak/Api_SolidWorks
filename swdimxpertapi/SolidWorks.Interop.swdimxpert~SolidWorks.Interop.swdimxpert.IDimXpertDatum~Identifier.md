<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDatum~Identifier.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| Identifier Property (IDimXpertDatum) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertDatum Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDatum.html) : Identifier Property (IDimXpertDatum) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the label for this DimXpert datum.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property Identifier As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertDatum Dim value As System.String   value = instance.Identifier ``` | |

| C# |  |
| --- | --- |
| ``` System.string Identifier {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ Identifier {    System.String^ get(); } ``` | |

#### Property Value

A label for the datum

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertDatum::Identifier.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Datum Example (C#)](Get_and_Set_Datum_Example_CSharp.htm)

[Get and Set Datum Example (VB.NET)](Get_and_Set_Datum_Example_VBNET.htm)

[Get and Set Datum Example (VBA)](Get_and_Set_Datum_Example_VB.htm)

[Get DimXpert Datum Example (VBA)](Get_DimXpert_Datum_Example_VB.htm)

[Get DimXpert Datum Example (VB.NET)](Get_DimXpert_Datum_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertDatum Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDatum.html)

[IDimXpertDatum Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertDatum_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0