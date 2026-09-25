<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption~NeedSuppress.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| NeedSuppress Property (ISwDMExternalReferenceOption) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMExternalReferenceOption Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption.html) : NeedSuppress Property (ISwDMExternalReferenceOption) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets whether to retrieve information about suppressed external references in the document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property NeedSuppress As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMExternalReferenceOption Dim value As System.Boolean   instance.NeedSuppress = value   value = instance.NeedSuppress ``` | |

| C# |  |
| --- | --- |
| ``` System.bool NeedSuppress {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool NeedSuppress {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True to retrieve suppressed references, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMExternalReferenceOption::NeedSuppress.

# ![](dotnetimages/collapse.gif)Example

[Get External References (VB.NET)](Get_External_References_Example_VBNET.htm)

[Get External References (C#)](Get_External_References_Example_CSharp.htm)

[Get Current Name of Configuration of Suppressed Component (VB.NET)](Get_Current_Name_of_Configuration_of_Suppressed_Component_Example_VBNET.htm)

[Get Current Name of Configuration of Suppressed Component (C#)](Get_Current_Name_of_Configuration_of_Suppressed_Component_Example_CSharp.htm)

[Get External References for Part (C#)](Get_External_References_for_Part_Example_CSharp.htm)

[Get External References for Part (VB.NET)](Get_External_References_for_Part_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

To find out if a reference is suppressed:

1. Call [ISwDMComponent6::PathName](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMComponent6~PathName.html) to set the component returned by [ISwDMDocument15::GetExternalFeatureReferences](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument15~GetExternalFeatureReferences.html).- Call [ISwDMComponent::IsSuppressed](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMComponent~IsSuppressed.html).

The suppression states of all of the external references are also stored in the parent document. To obtain this information in XML format, call [ISwDMDocument::GetXMLStream](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~GetXmlStream.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMExternalReferenceOption Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption.html)

[ISwDMExternalReferenceOption Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMExternalReferenceOption_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2011 SP0