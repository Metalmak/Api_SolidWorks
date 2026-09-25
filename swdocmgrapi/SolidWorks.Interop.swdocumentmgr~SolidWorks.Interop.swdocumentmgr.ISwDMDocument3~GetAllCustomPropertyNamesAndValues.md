<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument3~GetAllCustomPropertyNamesAndValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetAllCustomPropertyNamesAndValues Method (ISwDMDocument3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument3 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument3.html) : GetAllCustomPropertyNamesAndValues Method (ISwDMDocument3) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*names*
:   Array of Property Names

*types*
:   Array of Types

*linkedTo*
:   Array of linked to Values/Text Expressions (see Remarks)

*values*
:   Array of Evaluated Values

Gets all of the custom properties for this document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetAllCustomPropertyNamesAndValues( _    ByRef names As System.Object, _    ByRef types As System.Object, _    ByRef linkedTo As System.Object, _    ByRef values As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument3 Dim names As System.Object Dim types As System.Object Dim linkedTo As System.Object Dim values As System.Object   instance.GetAllCustomPropertyNamesAndValues(names, types, linkedTo, values) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAllCustomPropertyNamesAndValues(     out System.object names,    out System.object types,    out System.object linkedTo,    out System.object values ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAllCustomPropertyNamesAndValues(  &   [Out] System.Object^ names, &   [Out] System.Object^ types, &   [Out] System.Object^ linkedTo, &   [Out] System.Object^ values ) ``` | |

#### Parameters

*names*
:   Array of Property Names

*types*
:   Array of Types

*linkedTo*
:   Array of linked to Values/Text Expressions (see Remarks)

*values*
:   Array of Evaluated Values

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument3::GetAllCustomPropertyNamesAndValues.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If the properties are...** | **Then this method returns...** |
| Linked | The evaluated results of linkedTo |
| Not linked | Empty strings.  This method returns the same values as returned by [ISwDMDocument::GetCustomProperty](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~GetCustomProperty.html) |

This method returns evaluated values from when the document was last saved in SOLIDWORKS.

If you called [ISwDMDocument::SetCustomProperty](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~SetCustomProperty.html) to set a linked custom property, then you must open and save the file in SOLIDWORKS before calling this method. SOLIDWORKS must process the linked custom property before your DocumentMgr application can retrieve its evaluated value.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument3 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument3.html)

[ISwDMDocument3 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument3_members.html)

[ISwDMDocument::DeleteCustomProperty Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~DeleteCustomProperty.html)

[ISwDMDocument::GetCustomPropertyCount Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~GetCustomPropertyCount.html)

[ISwDMDocument::GetCustomPropertyNames Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~GetCustomPropertyNames.html)

[ISwDMConfiguration4::GetAllCustomPropertyNamesAndValues Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration4~GetAllCustomPropertyNamesAndValues.html)

[ISwDMDocument5::GetCustomPropertyValues Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument5~GetCustomPropertyValues.html)

[ISwDMDocument17::GetCustomProperty2 Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument17~GetCustomProperty2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2004 SP4