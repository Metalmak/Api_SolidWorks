<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7~GetComputedBOM.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetComputedBOM Method (IEdmFile7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html) : GetComputedBOM Method (IEdmFile7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oBomLayoutNameOrID*
:   Name or ID of a Bill of Materials layout (see **Remarks**)

*lVersionNo*
:   Version of file for which to get the Bill of Materials; 0 or -1 to use the latest version

*bsConfiguration*
:   Name of the file configuration

*lEdmBomFlags*
:   Combination of [EdmBomFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomFlag.html) bits

Gets an interface to a computed Bill of Materials.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetComputedBOM( _    ByVal oBomLayoutNameOrID As System.Object, _    ByVal lVersionNo As System.Integer, _    ByVal bsConfiguration As System.String, _    ByVal lEdmBomFlags As System.Integer _ ) As EdmBomView ``` | |

| C# |  |
| --- | --- |
| ``` EdmBomView GetComputedBOM(     System.object oBomLayoutNameOrID,    System.int lVersionNo,    System.string bsConfiguration,    System.int lEdmBomFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmBomView^ GetComputedBOM(  &   System.Object^ oBomLayoutNameOrID, &   System.int lVersionNo, &   System.String^ bsConfiguration, &   System.int lEdmBomFlags ) ``` | |

#### Parameters

*oBomLayoutNameOrID*
:   Name or ID of a Bill of Materials layout (see **Remarks**)

*lVersionNo*
:   Version of file for which to get the Bill of Materials; 0 or -1 to use the latest version

*bsConfiguration*
:   Name of the file configuration

*lEdmBomFlags*
:   Combination of [EdmBomFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomFlag.html) bits

#### Return Value

[IEdmBomView](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFile7](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To specify oBomLayoutNameOrID, use [IEdmBomMgr.GetBomLayouts](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr~GetBomLayouts.html) to enumerate the existing Bill of Materials layouts.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7.html)

[IEdmFile7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009