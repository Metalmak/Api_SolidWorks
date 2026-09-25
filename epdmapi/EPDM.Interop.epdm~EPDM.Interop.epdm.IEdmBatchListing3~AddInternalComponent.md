<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3~AddInternalComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddInternalComponent Method (IEdmBatchListing3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchListing3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3.html) : AddInternalComponent Method (IEdmBatchListing3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oPath*
:   Path of internal component

*oID*
:   ID of internal component

*oVirtualFileParentPath*
:   Path of parent folder

*oFileDate*
:   Date of file

*lParam*
:   User-defined argument

*bsConfigName*
:   Name of the configuration file from which to read variables

*lEdmListFileFlags*
:   Combination of [EdmListFileFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFileFlags.html) bits

Adds the specified internal component to the batch for listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddInternalComponent( _    ByVal oPath As System.Object, _    ByVal oID As System.Object, _    ByVal oVirtualFileParentPath As System.Object, _    ByVal oFileDate As System.Date, _    ByVal lParam As System.Integer, _    Optional ByVal bsConfigName As System.String, _    Optional ByVal lEdmListFileFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddInternalComponent(     System.object oPath,    System.object oID,    System.object oVirtualFileParentPath,    System.DateTime oFileDate,    System.int lParam,    System.string bsConfigName,    System.int lEdmListFileFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddInternalComponent(  &   System.Object^ oPath, &   System.Object^ oID, &   System.Object^ oVirtualFileParentPath, &   System.DateTime oFileDate, &   System.int lParam, &   System.String^ bsConfigName, &   System.int lEdmListFileFlags ) ``` | |

#### Parameters

*oPath*
:   Path of internal component

*oID*
:   ID of internal component

*oVirtualFileParentPath*
:   Path of parent folder

*oFileDate*
:   Date of file

*lParam*
:   User-defined argument

*bsConfigName*
:   Name of the configuration file from which to read variables

*lEdmListFileFlags*
:   Combination of [EdmListFileFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmListFileFlags.html) bits

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchListing3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3.html)

[IEdmBatchListing3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010