<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~Clone.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Clone Method (IEdmPos5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmPos5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) : Clone Method (IEdmPos5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Creates a copy of an IEdmPos5 object.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function Clone() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 Clone() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ Clone(); ``` | |

#### Return Value

Copy of an [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html) object

# ![](dotnetimages/collapse.gif)Remarks

C++ users must release the returned pointer.

You can use a copy of an IEdmPos5 object as a bookmark in an enumeration that you are performing with this object.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmPos5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html)

[IEdmPos5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional