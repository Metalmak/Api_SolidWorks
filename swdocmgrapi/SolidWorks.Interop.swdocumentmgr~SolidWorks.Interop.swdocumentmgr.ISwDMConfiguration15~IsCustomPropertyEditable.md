<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15~IsCustomPropertyEditable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| IsCustomPropertyEditable Method (ISwDMConfiguration15) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration15 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15.html) : IsCustomPropertyEditable Method (ISwDMConfiguration15) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FieldName*
:   Name of the custom property (see **Remarks**)

*IsEditable*
:   True if editable, false if not

Gets whether the specified custom property is editable.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IsCustomPropertyEditable( _    ByVal FieldName As System.String, _    ByRef IsEditable As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration15 Dim FieldName As System.String Dim IsEditable As System.Boolean   instance.IsCustomPropertyEditable(FieldName, IsEditable) ``` | |

| C# |  |
| --- | --- |
| ``` void IsCustomPropertyEditable(     System.string FieldName,    out System.bool IsEditable ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IsCustomPropertyEditable(  &   System.String^ FieldName, &   [Out] System.bool IsEditable ) ``` | |

#### Parameters

*FieldName*
:   Name of the custom property (see **Remarks**)

*IsEditable*
:   True if editable, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration15::IsCustomPropertyEditable.

# ![](dotnetimages/collapse.gif)Remarks

To populate FieldName, use [ISwDMConfiguration::GetCustomPropertyNames](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration~GetCustomPropertyNames.html) to get the names of all of the custom properties.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration15 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15.html)

[ISwDMConfiguration15 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration15_members.html)

[ISwDMConfiguration14::GetCustomProperty2 Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration14~GetCustomProperty2.html)

[ISwDMConfiguration4::GetAllCustomPropertyNamesAndValues Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration4~GetAllCustomPropertyNamesAndValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2018 SP0