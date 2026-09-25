<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateDeformedBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateDeformedBody Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : CreateDeformedBody Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NCreateAs*
:   Save option as defined in [swsCreateDeformedBodyOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyOption_e.html)

*SName*
:   Name of the part or configuration to save

*ErrorCode*
:   Error code as defined in [swsCreateDeformedBodyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyError_e.html)

Obsolete. Superseded by [ICWResults::CreateDeformedBody2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~CreateDeformedBody2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub CreateDeformedBody( _    ByVal NCreateAs As System.Integer, _    ByVal SName As System.String, _    ByRef ErrorCode As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NCreateAs As System.Integer Dim SName As System.String Dim ErrorCode As System.Integer   instance.CreateDeformedBody(NCreateAs, SName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` void CreateDeformedBody(     System.int NCreateAs,    System.string SName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CreateDeformedBody(  &   System.int NCreateAs, &   System.String^ SName, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NCreateAs*
:   Save option as defined in [swsCreateDeformedBodyOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyOption_e.html)

*SName*
:   Name of the part or configuration to save

*ErrorCode*
:   Error code as defined in [swsCreateDeformedBodyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCreateDeformedBodyError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::CreateDeformedBody.

# ![](dotnetimages/collapse.gif)Remarks

The new document is saved in the location of the original part or assembly.

Deformed shapes of assembly documents are saved as multibody parts.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetDeformedBodyFailedSewOption Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetDeformedBodyFailedSewOption.html)

[ICWResults::SetDeformedBodyFailedSewOption Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~SetDeformedBodyFailedSewOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0