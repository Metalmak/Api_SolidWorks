<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx~mbsPicturePath.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| mbsPicturePath Field | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [EdmUserDataEx Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html) : mbsPicturePath Field |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Points to an image file (e.g., **.jpg**, **.bmp**, **.png**, etc.)  that can be set using [IEdmUser10::SetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~SetUserDataEx.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public mbsPicturePath As System.String ``` | |

| C# |  |
| --- | --- |
| ``` public System.string mbsPicturePath ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public: System.String^ mbsPicturePath ``` | |

# ![](dotnetimages/collapse.gif)Remarks

The member can be set to an empty or null string to remove the user's picture.

If you call [IEdmUser10::GetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~GetUserDataEx.html), then this field points to the user's picture cached to the client computer disk. This is the cache used bySOLIDWORKS PDM Professional, so you should not delete the file from that location.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmUserDataEx Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx.html)

[EdmUserDataEx Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserDataEx_members.html)