<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument~GetXmlStream.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetXmlStream Method (ISwDMDocument) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument.html) : GetXmlStream Method (ISwDMDocument) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*xmlFileName*
:   Filename for the XML document

*result*
:   Success or error code as defined by [SwDMXmlDataError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmXmlDataError.html)

Gets the embedded XML data for this assembly and saves it to an XML document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetXmlStream( _    ByVal xmlFileName As System.String, _    ByRef result As SwDmXmlDataError _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument Dim xmlFileName As System.String Dim result As SwDmXmlDataError   instance.GetXmlStream(xmlFileName, result) ``` | |

| C# |  |
| --- | --- |
| ``` void GetXmlStream(     System.string xmlFileName,    ref SwDmXmlDataError result ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetXmlStream(  &   System.String^ xmlFileName, &   SwDmXmlDataError% result ) ``` | |

#### Parameters

*xmlFileName*
:   Filename for the XML document

*result*
:   Success or error code as defined by [SwDMXmlDataError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmXmlDataError.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument::GetXmlStream.

# ![](dotnetimages/collapse.gif)Example

[Get XML Stream (C#)](Get_XML_Stream_Example_CSharp.htm)

[Get XML Stream (VB.NET)](Get_XML_Stream_Example_VBNET.htm)

[Get External References for Part (C#)](Get_External_References_for_Part_Example_CSharp.htm)

[Get External References for Part (VB.NET)](Get_External_References_for_Part_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only returns data for documents created using SOLIDWORKS 2003 (Version 2200) and later. To get the version of a document, use [ISwDMDocument::GetVersion](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~GetVersion.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument.html)

[ISwDMDocument Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2004 FCS