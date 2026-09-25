<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr7~GetDrawingPropSheetAttributes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetDrawingPropSheetAttributes Method (IEdmVariableMgr7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVariableMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr7.html) : GetDrawingPropSheetAttributes Method (IEdmVariableMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of folder from which to get the values

*ppoSrcAttribs*
:   Array of attribute names used in the CustomProperty block

*ppoDestAttribs*
:   Array of attribute names used in the $PRPSheet block

Gets all of the SLDDRW-card attributes that are linked to the $PRPSHEET block for the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetDrawingPropSheetAttributes( _    ByVal lFolderID As System.Integer, _    ByRef ppoSrcAttribs() As System.String, _    ByRef ppoDestAttribs() As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDrawingPropSheetAttributes(     System.int lFolderID,    out System.string[] ppoSrcAttribs,    out System.string[] ppoDestAttribs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDrawingPropSheetAttributes(  &   System.int lFolderID, &   [Out] System.array<String^>^ ppoSrcAttribs, &   [Out] System.array<String^>^ ppoDestAttribs ) ``` | |

#### Parameters

*lFolderID*
:   ID of folder from which to get the values

*ppoSrcAttribs*
:   Array of attribute names used in the CustomProperty block

*ppoDestAttribs*
:   Array of attribute names used in the $PRPSheet block

# ![](dotnetimages/collapse.gif)Remarks

This method is used internally by SOLIDWORKS PDM Professional to copy attributes from the model's CustomProperty block to the $PRPSHEET block. ppoSrcAttribs and ppoDestAttribs both have the same number of elements.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVariableMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr7.html)

[IEdmVariableMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011