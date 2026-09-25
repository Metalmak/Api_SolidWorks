<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_DynamicHighlightNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_DynamicHighlightNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_DynamicHighlightNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*bHighlightState*
:   True if highlighting is on, false if it is off

Post-notifies the application when dynamic highlighting of the selected object changes from on to off, and vice versa.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_DynamicHighlightNotifyEventHandler( _    ByVal bHighlightState As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_DynamicHighlightNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_DynamicHighlightNotifyEventHandler(     System.bool bHighlightState ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_DynamicHighlightNotifyEventHandler(  &   System.bool bHighlightState ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*bHighlightState*
:   True if highlighting is on, false if it is off

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DynamicHighlightNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Example

Private Function drawdoc\_DynamicHighlightNotify() As Long

Dim one As Object

Dim x As Integer

Dim pt As Variant

Set one = mgr.GetSelectedObject5(-1)

If Not one Is Nothing Then

    Debug.Print mgr.GetSelectedObjectType2(-1)

    one.Select True

    pt = mgr.GetSelectionPoint(-1)

    If Not IsEmpty(pt) Then

        Debug.Print pt(0), pt(1), pt(2)

    Else

        Debug.Print "Object selected in FeatureManager design tree, so no points."

    End If

Else

    Debug.Print "Dynamic highlighting is now off."

End If

# ![](dotnetimages/collapse.gif)Remarks

To send this notification, specify -1 for the index for any of the [ISelectionMgr](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectionMgr.html) methods. See **Example**.

If developing a C++ application, use swDrawingDynamicHighlightNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0