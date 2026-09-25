<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin~DisconnectFromSW.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| DisconnectFromSW Method (ISwAddin) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwAddin Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin.html) : DisconnectFromSW Method (ISwAddin) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Calls this method when SOLIDWORKS is about to be destroyed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DisconnectFromSW() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddin Dim value As System.Boolean   value = instance.DisconnectFromSW() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DisconnectFromSW() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DisconnectFromSW(); ``` | |

#### Return Value

True if the add-in disconnected successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddin::DisconnectFromSW.

# ![](dotnetimages/collapse.gif)Remarks

This is a pre-notification. Add-ins should perform any clean up inside this event.

When this method is called, remove and release all user-interface items related to this add-in (for example, menus, and toolbars).

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddin Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin.html)

[ISwAddin Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0