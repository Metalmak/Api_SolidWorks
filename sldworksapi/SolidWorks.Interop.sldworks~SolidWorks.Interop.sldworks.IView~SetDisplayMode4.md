<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetDisplayMode4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDisplayMode4 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : SetDisplayMode4 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseParent*
:   True to use the parent's settings, false to use this drawing view's local settings (see **Remarks**)

*Mode*
:   Display mode of the drawing view as defined in swDisplayMode\_e (see **Remarks**)

*Faceted*
:   True for draft quality, false for precision quality (see **Remarks**)

*Edges*
:   True if edges are displayed when this view is in shaded mode, false if not

*CThreadHighQuality*
:   True for precision quality cosmetic threads, false for draft quality

Sets the display mode of this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDisplayMode4( _    ByVal UseParent As System.Boolean, _    ByVal Mode As System.Integer, _    ByVal Faceted As System.Boolean, _    ByVal Edges As System.Boolean, _    ByVal CThreadHighQuality As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim UseParent As System.Boolean Dim Mode As System.Integer Dim Faceted As System.Boolean Dim Edges As System.Boolean Dim CThreadHighQuality As System.Boolean Dim value As System.Boolean   value = instance.SetDisplayMode4(UseParent, Mode, Faceted, Edges, CThreadHighQuality) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDisplayMode4(     System.bool UseParent,    System.int Mode,    System.bool Faceted,    System.bool Edges,    System.bool CThreadHighQuality ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDisplayMode4(  &   System.bool UseParent, &   System.int Mode, &   System.bool Faceted, &   System.bool Edges, &   System.bool CThreadHighQuality ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseParent*
:   True to use the parent's settings, false to use this drawing view's local settings (see **Remarks**)

*Mode*
:   Display mode of the drawing view as defined in swDisplayMode\_e (see **Remarks**)

*Faceted*
:   True for draft quality, false for precision quality (see **Remarks**)

*Edges*
:   True if edges are displayed when this view is in shaded mode, false if not

*CThreadHighQuality*
:   True for precision quality cosmetic threads, false for draft quality

#### Return Value

True if the display mode is reset, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::SetDisplayMode4.

# ![](dotnetimages/collapse.gif)Example

'VBA

'-------------------------------------
' Preconditions:
' 1. Open a drawing and select a drawing view.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Gets the selected view's current display mode properties.
' 2. Resets the display mode properties.
' 3. Gets the new display mode properties.
' 4. Examine the Immediate window.
'--------------------------------------

Option Explicit
Sub main()

    Dim swApp As SldWorks.SldWorks
    Dim swModel As SldWorks.ModelDoc2
    Dim swDraw As SldWorks.DrawingDoc
    Dim swSheet As SldWorks.Sheet
    Dim swView As SldWorks.View
    Dim bRet As Boolean
    Dim swSelectionMgr As SldWorks.SelectionMgr

    Set swApp = SolidWorks.SldWorks
    Set swModel = swApp.ActiveDoc
    Set swDraw = swModel
    Set swSheet = swDraw.GetCurrentSheet
    Set swSelectionMgr = swModel.SelectionManager

    Set swView = swSelectionMgr.GetSelectedObject6(1, -1)

    Debug.Print "=====Current Display Mode======"
    Debug.Print ""

    Dim UseParentProp As Boolean
    UseParentProp = swView.**GetUseParentDisplayMode**
    Debug.Print "Using parent view's display mode?  " & UseParentProp

    Dim displayMode As Long
    displayMode = swView.**GetDisplayMode2**
    Debug.Print "Current display mode as defined by swDisplayMode\_e:  " & displayMode

    Dim Faceted As Boolean
    Faceted = swView.**GetFacettedHlrDisplay**
    Debug.Print "Display faceted?:  " & Faceted

    Dim EdgesMode As Boolean
    EdgesMode = swView.**GetDisplayEdgesInShadedMode**
    Debug.Print "Display edges when the view is in shaded mode?  " & EdgesMode

    Dim cThreadQuality As Boolean
    cThreadQuality = swView.**GetCThreadQuality**
    Debug.Print "Precision quality for cosmetic threads? " & swView.GetCThreadQuality

    swView.**SetDisplayMode4** False, 3, True, False, True

    Debug.Print "=====After Re-setting Display Mode======"
    Debug.Print ""
    Debug.Print "Using parent view's display mode?  " & swView.**GetUseParentDisplayMode**
    Debug.Print "Current display mode as defined by swDisplayMode\_e:  " & swView.**GetDisplayMode2**
    Debug.Print "Display faceted?  " & swView.**GetFacettedHlrDisplay**
    Debug.Print "Display edges when the view is in shaded mode?  " & swView.**GetDisplayEdgesInShadedMode**
    Debug.Print "Precision quality for cosmetic threads? " & swView.**GetCThreadQuality**

End Sub

# ![](dotnetimages/collapse.gif)Example

[Set Display Mode of View (VB.NET)](Set_Display_Mode_of_View_Example_VBNET.htm)

[Set Display Mode of View (C#)](Set_Display_Mode_of_View_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If UseParent is true and a parent view:

* Exists, then this method's Mode, Faceted, and Edges parameters are ignored.* Does not exist, then this method does not change the current display mode of this drawing view.

Mode specifies the drawing view display as defined by swDisplayMode\_e.:

* swWIREFRAME* swHIDDEN (Hidden Lines Removed)* swHIDDEN\_GREYED (Hidden Lines Visible)* swSHADED* swSHADED\_EDGES

swDisplayMode\_e also contains three other values that seem to indicate faceted (draft) geometry:

* swFACETED\_WIREFRAME* swFACETED\_HIDDEN\_GREYED* swFACETED\_HIDDEN

However in this method, you must use the Faceted parameter (not the Mode parameter) to specify draft or precision quality. If you specify Mode with swFACETED\_WIREFRAME, swFACETED\_HIDDEN\_GREYED, or swFACETED\_HIDDEN, then SOLIDWORKS instead uses swWIREFRAME, swHIDDEN\_GREYED, or swHIDDEN.

NOTE: Just as displaying geometry precisely can decrease performance, setting the Faceted argument to true (draft quality) can increase performance.

|  |  |
| --- | --- |
| **To determine for this view...** | **Use...** |
| Whether its edges are displayed when it's in shaded mode | [IView::GetDisplayEdgesInShadedMode](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetDisplayEdgesInShadedMode.html) |
| Whether its geometry is faceted | [IView::GetFacettedHlrDisplay](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFacettedHlrDisplay.html) |
| Its current display mode | [IView::GetDisplayMode2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetDisplayMode2.html) |
| Whether its parent's display mode is being used | [IView::GetUseParentDisplayMode](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetUseParentDisplayMode.html) |
| Its cosmetic thread display quality | [IView::GetCThreadQuality](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetCThreadQuality.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29