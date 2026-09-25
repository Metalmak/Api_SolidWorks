<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard7~GetAllControls.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAllControls Method (IEdmCard7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCard7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard7.html) : GetAllControls Method (IEdmCard7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppControlsList*
:   Array of [IEdmCardControl5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

Gets all controls in this file or folder data card.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetAllControls( _    ByRef ppControlsList() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAllControls(     out System.object[] ppControlsList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAllControls(  &   [Out] System.array<Object^>^ ppControlsList ) ``` | |

#### Parameters

*ppControlsList*
:   Array of [IEdmCardControl5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCard7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard7.html) example.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCard7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard7.html)

[IEdmCard7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2019 SP03