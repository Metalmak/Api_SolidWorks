<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6~SetProgressRange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetProgressRange Method (IEdmCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) : SetProgressRange Method (IEdmCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lBarIndex*
:   0-based index of the progress bar

*lMax*
:   Maximum value for the progress bar; minimum value is always 0

Sets the maximum value for a progress bar.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetProgressRange( _    ByVal lBarIndex As System.Integer, _    ByVal lMax As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProgressRange(     System.int lBarIndex,    System.int lMax ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProgressRange(  &   System.int lBarIndex, &   System.int lMax ) ``` | |

#### Parameters

*lBarIndex*
:   0-based index of the progress bar

*lMax*
:   Maximum value for the progress bar; minimum value is always 0

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* <any error code>: The calling method terminated.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html)

[IEdmCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0