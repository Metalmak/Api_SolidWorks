<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22~IsCustomPropertyEditable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| IsCustomPropertyEditable Method (ISwDMDocument22) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument22 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22.html) : IsCustomPropertyEditable Method (ISwDMDocument22) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FieldName*
:   Name of the custom property in this document

*IsEditable*
:   True if editable, false if not

Gets whether the specified custom property is editable.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IsCustomPropertyEditable( _    ByVal FieldName As System.String, _    ByRef IsEditable As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument22 Dim FieldName As System.String Dim IsEditable As System.Boolean   instance.IsCustomPropertyEditable(FieldName, IsEditable) ``` | |

| C# |  |
| --- | --- |
| ``` void IsCustomPropertyEditable(     System.string FieldName,    out System.bool IsEditable ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IsCustomPropertyEditable(  &   System.String^ FieldName, &   [Out] System.bool IsEditable ) ``` | |

#### Parameters

*FieldName*
:   Name of the custom property in this document

*IsEditable*
:   True if editable, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument22::IsCustomPropertyEditable.

# ![](dotnetimages/collapse.gif)Example

See the [ISwDMDocument22](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To populate FieldName, use [ISwDMDocument::GetCustomPropertyNames](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~GetCustomPropertyNames.html) to get the names of all of the custom properties in this document.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument22 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22.html)

[ISwDMDocument22 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument22_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2018 SP0