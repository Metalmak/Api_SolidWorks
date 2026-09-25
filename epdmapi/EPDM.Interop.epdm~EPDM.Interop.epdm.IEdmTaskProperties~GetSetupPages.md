<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetSetupPages.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSetupPages Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : GetSetupPages Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoPages*
:   Array of [EdmTaskSetupPage](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage.html) structures; one structure for each setup page

Gets the setup pages added to the task property dialog box using [IEdmTaskProperties::SetSetupPages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetSetupPages.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetSetupPages( _    ByRef ppoPages() As EdmTaskSetupPage _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSetupPages(     out EdmTaskSetupPage[] ppoPages ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSetupPages(  &   [Out] array<EdmTaskSetupPage>^ ppoPages ) ``` | |

#### Parameters

*ppoPages*
:   Array of [EdmTaskSetupPage](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskSetupPage.html) structures; one structure for each setup page

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010