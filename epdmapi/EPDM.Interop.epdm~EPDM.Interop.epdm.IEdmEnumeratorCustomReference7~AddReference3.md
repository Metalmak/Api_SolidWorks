<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7~AddReference3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddReference3 Method (IEdmEnumeratorCustomReference7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorCustomReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html) : AddReference3 Method (IEdmEnumeratorCustomReference7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

*lQuantity*
:   Number of times the referenced file is referenced

*bShowInBOM*
:   True to show this file reference in the BOM, false to not

Adds a custom file reference to this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddReference3( _    ByVal lFileID As System.Integer, _    ByVal lFolderID As System.Integer, _    ByVal lQuantity As System.Integer, _    Optional ByVal bShowInBOM As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddReference3(     System.int lFileID,    System.int lFolderID,    System.int lQuantity,    System.bool bShowInBOM ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddReference3(  &   System.int lFileID, &   System.int lFolderID, &   System.int lQuantity, &   System.bool bShowInBOM ) ``` | |

#### Parameters

*lFileID*
:   ID of referenced file

*lFolderID*
:   ID of parent folder of referenced file

*lQuantity*
:   Number of times the referenced file is referenced

*bShowInBOM*
:   True to show this file reference in the BOM, false to not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmEnumeratorCustomReference7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU: File is not checked out.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorCustomReference7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7.html)

[IEdmEnumeratorCustomReference7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorCustomReference7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017