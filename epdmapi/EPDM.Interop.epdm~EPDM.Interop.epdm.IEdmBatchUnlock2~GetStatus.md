<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock2~GetStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetStatus Method (IEdmBatchUnlock2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUnlock2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock2.html) : GetStatus Method (IEdmBatchUnlock2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmUnlockStatusFlag*
:   Combination of [EdmUnlockStatusFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockStatusFlag.html) bits

Gets the specified statuses for this unlock operation.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetStatus( _    ByVal lEdmUnlockStatusFlag As System.Integer _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetStatus(     System.int lEdmUnlockStatusFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetStatus(  &   System.int lEdmUnlockStatusFlag ) ``` | |

#### Parameters

*lEdmUnlockStatusFlag*
:   Combination of [EdmUnlockStatusFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUnlockStatusFlag.html) bits

#### Return Value

Array of statuses

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUnlock2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock2.html)

[IEdmBatchUnlock2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013