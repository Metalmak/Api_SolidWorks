<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ShowSmartMessage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowSmartMessage Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ShowSmartMessage Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Message to display in the ToolTip

*TimeInMillSec*
:   Time, in milliseconds, to display the message

*ShowInStatusBar*
:   True to show the message on the SOLIDWORKS status bar, false to not

*RemoveDefaultTip*
:   True to replace the default SOLIDWORKS ToolTip with this message for TimeInMillSec, false to not

Displays a SOLIDWORKS-style message as a ToolTip in the graphics area and on the status bar.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowSmartMessage( _    ByVal Name As System.String, _    ByVal TimeInMillSec As System.Integer, _    ByVal ShowInStatusBar As System.Boolean, _    ByVal RemoveDefaultTip As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Name As System.String Dim TimeInMillSec As System.Integer Dim ShowInStatusBar As System.Boolean Dim RemoveDefaultTip As System.Boolean   instance.ShowSmartMessage(Name, TimeInMillSec, ShowInStatusBar, RemoveDefaultTip) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowSmartMessage(     System.string Name,    System.int TimeInMillSec,    System.bool ShowInStatusBar,    System.bool RemoveDefaultTip ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowSmartMessage(  &   System.String^ Name, &   System.int TimeInMillSec, &   System.bool ShowInStatusBar, &   System.bool RemoveDefaultTip ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Message to display in the ToolTip

*TimeInMillSec*
:   Time, in milliseconds, to display the message

*ShowInStatusBar*
:   True to show the message on the SOLIDWORKS status bar, false to not

*RemoveDefaultTip*
:   True to replace the default SOLIDWORKS ToolTip with this message for TimeInMillSec, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ShowSmartMessage.

# ![](dotnetimages/collapse.gif)Example

**Visual Basic for Applications (VBA):**

Option Explicit

Dim swApp As SldWorks.SldWorks
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim swModel As SldWorks.ModelDoc2
Dim swSelMgr As SldWorks.SelectionMgr

Sub main()

Set swApp = Application.SldWorks
Set swModel = swApp.**ActiveDoc**
swModel.**ClearSelection2** True
Set swSelMgr = swModel.**SelectionManager**
Set swModelDocExt = swModel.**Extension**
While 1

' Loops until you select an entity in the graphics area

While swSelMgr.**GetSelectedObjectCount** = 0
DoEvents
Wend

swModelDocExt.**ShowSmartMessage** "This is the message.", 500, True, True
DoEvents
Wend

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0