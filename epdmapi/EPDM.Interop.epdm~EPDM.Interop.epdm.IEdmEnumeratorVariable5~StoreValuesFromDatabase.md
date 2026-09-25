<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5~StoreValuesFromDatabase.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| StoreValuesFromDatabase Method (IEdmEnumeratorVariable5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html) : StoreValuesFromDatabase Method (IEdmEnumeratorVariable5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of the file's parent folder

*bOnlyMissingValues*
:   True to only copy variables without a value, false to copy all variables

*poProgressCb*
:   Not used

Copies file data card data from the SOLIDWORKS PDM Professional database to the file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub StoreValuesFromDatabase( _    ByVal lFolderID As System.Integer, _    ByVal bOnlyMissingValues As System.Boolean, _    Optional ByVal poProgressCb As EdmCallback _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void StoreValuesFromDatabase(     System.int lFolderID,    System.bool bOnlyMissingValues,    EdmCallback poProgressCb ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void StoreValuesFromDatabase(  &   System.int lFolderID, &   System.bool bOnlyMissingValues, &   EdmCallback^ poProgressCb ) ``` | |

#### Parameters

*lFolderID*
:   ID of the file's parent folder

*bOnlyMissingValues*
:   True to only copy variables without a value, false to copy all variables

*poProgressCb*
:   Not used

# ![](dotnetimages/collapse.gif)Remarks

This method corresponds to the SOLIDWORKS PDM Professional user interface right-click menu command, Update File Attributes from Database.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_FILE: The file format is not recognized.* E\_EDM\_FILE\_SHARE\_ERROR: The file is exclusively opened in another application.* E\_EDM\_IO\_ERROR: Error writing data to the file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5.html)

[IEdmEnumeratorVariable5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2