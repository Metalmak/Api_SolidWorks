<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin~ConnectToSW.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| ConnectToSW Method (ISwAddin) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwAddin Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin.html) : ConnectToSW Method (ISwAddin) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ThisSW*
:   Pointer to the SldWorks Dispatch object

*Cookie*
:   Add-in ID

Calls this method when the add-in is loaded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConnectToSW( _    ByVal ThisSW As System.Object, _    ByVal Cookie As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddin Dim ThisSW As System.Object Dim Cookie As System.Integer Dim value As System.Boolean   value = instance.ConnectToSW(ThisSW, Cookie) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ConnectToSW(     System.object ThisSW,    System.int Cookie ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ConnectToSW(  &   System.Object^ ThisSW, &   System.int Cookie ) ``` | |

#### Parameters

*ThisSW*
:   Pointer to the SldWorks Dispatch object

*Cookie*
:   Add-in ID

#### Return Value

True if the add-in connected successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddin::ConnectToSW.

# ![](dotnetimages/collapse.gif)Remarks

When this method is called, add all required items for this add-in to the SOLIDWORKS user interface (for example, menus and toolbars) and set the event handler.

ISldWorks::ExitApp does not work if called from within this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddin Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin.html)

[ISwAddin Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0