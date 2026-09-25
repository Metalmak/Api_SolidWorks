<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9~GetObjects.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetObjects Method (IEdmVault9) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9.html) : GetObjects Method (IEdmVault9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoObjects*
:   Array of [EdmObjectInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo.html) structures; one structure for each interface to retrieve

Gets interfaces to all of the specified objects.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetObjects( _    ByRef ppoObjects() As EdmObjectInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetObjects(     out EdmObjectInfo[] ppoObjects ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetObjects(  &   [Out] array<EdmObjectInfo>^ ppoObjects ) ``` | |

#### Parameters

*ppoObjects*
:   Array of [EdmObjectInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectInfo.html) structures; one structure for each interface to retrieve

# ![](dotnetimages/collapse.gif)Example

[Batch Update Card Variables (C#)](Batch_Update_Variables_Example_CSharp.htm)

[Batch Update Card Variables (VB.NET)](Batch_Update_Variables_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method to get interfaces to several objects at once, which is more efficient than calling [IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html) multiple times.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9.html)

[IEdmVault9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008