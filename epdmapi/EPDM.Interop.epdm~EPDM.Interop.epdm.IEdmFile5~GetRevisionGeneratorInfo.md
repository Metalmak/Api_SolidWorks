<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetRevisionGeneratorInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetRevisionGeneratorInfo Method (IEdmFile5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetRevisionGeneratorInfo Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*pbIncrementMenu*
:   True if there should be an Increment Revision menu item in the context menu of this file, false if not

Gets information about this file for the revision generator.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetRevisionGeneratorInfo( _    ByRef pbIncrementMenu As System.Boolean _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetRevisionGeneratorInfo(     out System.bool pbIncrementMenu ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetRevisionGeneratorInfo(  &   [Out] System.bool pbIncrementMenu ) ``` | |

#### Parameters

*pbIncrementMenu*
:   True if there should be an Increment Revision menu item in the context menu of this file, false if not

#### Return Value

True if there is a revision number generator set up for the file's current state in the workflow, false if not

# ![](dotnetimages/collapse.gif)Remarks

This method exists mainly for internal purposes.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_REV\_GEN\_LIST\_STOP: It is not possible to increment revision on this file, because SOLIDWORKS PDM Professional has reached the end of the revision list that was set up in the Workflow Editor.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2