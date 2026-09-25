<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~LoadXMLBuffer.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| LoadXMLBuffer Method (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : LoadXMLBuffer Method (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XMLDoc*
:   Pointer to the an MSXML DOMDocument object (MSXML2.DOMDocument40)

Loads the model from data from an XML source.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub LoadXMLBuffer( _    ByVal XMLDoc As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim XMLDoc As System.Object   instance.LoadXMLBuffer(XMLDoc) ``` | |

| C# |  |
| --- | --- |
| ``` void LoadXMLBuffer(     System.object XMLDoc ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LoadXMLBuffer(  &   System.Object^ XMLDoc ) ``` | |

#### Parameters

*XMLDoc*
:   Pointer to the an MSXML DOMDocument object (MSXML2.DOMDocument40)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::LoadXMLBuffer.

# ![](dotnetimages/collapse.gif)Example

<TITLE>eDrawings 2005 - [square]</TITLE><HTML>

<BODY>

<OBJECT ID="EV" classid="clsid:22945A69-1191-4DCF-9E6F-409BDE94D101" codebase="http://www.solidworks.com/plugins/edrawings/ " width="100%" height="99%"><PARAM name="FullUI" value="1"/></OBJECT>

<font color="#000000" face="Times, Verdana, Helvetica, Arial">Internet Explorer 5.5 or higher is required to view this <a href="http://www.solidworks.com/edrawings">eDrawings</a> file.      Generated with eDrawings 2005.</font>

<SCRIPT>function edwsc(){if(event.srcElement.readyState=="complete")EV.LoadXMLBuffer(event.srcElement.XMLDocument);}</SCRIPT>

<XML ID="EDW1" onreadystatechange="edwsc()">

<EDWData>

<!-- Embedded EDrawing data saved as text --!>  See IPDMWDocument::GetEmbeddedEDWAsBase64

</EDWData>

</XML>

</BODY>

</HTML>

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0