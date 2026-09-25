<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetPopupMenuMode.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPopupMenuMode Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetPopupMenuMode Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ModeIn*
:   Pop-up menu mode (see **Remarks**)

Sets the pop-up menu mode.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetPopupMenuMode( _    ByVal ModeIn As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ModeIn As System.Integer   instance.SetPopupMenuMode(ModeIn) ``` | |

| C# |  |
| --- | --- |
| ``` void SetPopupMenuMode(     System.int ModeIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetPopupMenuMode(  &   System.int ModeIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ModeIn*
:   Pop-up menu mode (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetPopupMenuMode.

# ![](dotnetimages/collapse.gif)Remarks

When end users press the right-mouse button on an entity in the graphics window, they are be presented with one of two menu sets. These menu sets are defined as mode 0 and mode 1.

**Mode**

* 0 - Default shortcut mode. This mode presents the end user with options to Select Other, manipulate the view, access the properties dialog of the selected item, and so on.

  * 1 - The end-user is presented with a limited set of choices including Select Other and Clear Selection. This mode is typically seen when a SOLIDWORKS dialog is active and the user is restricted to entity selection.

Using this method, you can simulate the same shortcut menu behavior as in the SOLIDWORKS user interface. If you have a dialog that requires user selection of entities, you can set the pop-up menu mode to 1 to simulate SOLIDWORKS behavior. Your application should always set the menu mode back to its previous value. To determine the previous behavior, call [IModelDoc2::GetPopupMenuMode](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GetPopupMenuMode.html) prior to calling to this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0