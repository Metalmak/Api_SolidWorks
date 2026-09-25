<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~AutoInsertCenterMarks2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutoInsertCenterMarks2 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : AutoInsertCenterMarks2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InsertType*
:   Features for which to insert center marks as defined in swAutoInsertCenterMarkTypes\_e

*InsertOption*
:   Center mark options as defined in swCenterMarkConnectionLine\_e

*LinearSlotCenter*
:   True to add center marks to slot centers, false to add them to slot ends

*ArcSlotCenter*
:   True to add center marks to arc centers, false to add them to arc ends

*UseDocumentDefaults*
:   True to use the display settings specified in **Tools > Options > Document Properties > Centerlines/Center Marks**, false to use the display settings set by this method

*Size*
:   Size of center mark; valid only if UseDocumentDefaults is false

*Gap*
:   Size of gap between the center mark and extension line; valid only if UseDocumentDefaults is false and the**Tools > Options > Document Properties > Centerlines/Center Marks > Scale by view scale** check box is clear (see **Remarks**)

*ExtendedLines*
:   True to extend lines from center mark points, false to not; valid only if UseDocumentDefaults is false

*CenterLineFont*
:   True to use the centerline font, false to not; valid only if UseDocumentDefaults is false

*Angle*
:   Rotation angle for the center mark; a positive angle rotates the center mark counterclockwise

Automatically inserts the specified center marks in this view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AutoInsertCenterMarks2( _    ByVal InsertType As System.Integer, _    ByVal InsertOption As System.Integer, _    ByVal LinearSlotCenter As System.Boolean, _    ByVal ArcSlotCenter As System.Boolean, _    ByVal UseDocumentDefaults As System.Boolean, _    ByVal Size As System.Double, _    ByVal Gap As System.Double, _    ByVal ExtendedLines As System.Boolean, _    ByVal CenterLineFont As System.Boolean, _    ByVal Angle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim InsertType As System.Integer Dim InsertOption As System.Integer Dim LinearSlotCenter As System.Boolean Dim ArcSlotCenter As System.Boolean Dim UseDocumentDefaults As System.Boolean Dim Size As System.Double Dim Gap As System.Double Dim ExtendedLines As System.Boolean Dim CenterLineFont As System.Boolean Dim Angle As System.Double Dim value As System.Boolean   value = instance.AutoInsertCenterMarks2(InsertType, InsertOption, LinearSlotCenter, ArcSlotCenter, UseDocumentDefaults, Size, Gap, ExtendedLines, CenterLineFont, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AutoInsertCenterMarks2(     System.int InsertType,    System.int InsertOption,    System.bool LinearSlotCenter,    System.bool ArcSlotCenter,    System.bool UseDocumentDefaults,    System.double Size,    System.double Gap,    System.bool ExtendedLines,    System.bool CenterLineFont,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AutoInsertCenterMarks2(  &   System.int InsertType, &   System.int InsertOption, &   System.bool LinearSlotCenter, &   System.bool ArcSlotCenter, &   System.bool UseDocumentDefaults, &   System.double Size, &   System.double Gap, &   System.bool ExtendedLines, &   System.bool CenterLineFont, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InsertType*
:   Features for which to insert center marks as defined in swAutoInsertCenterMarkTypes\_e

*InsertOption*
:   Center mark options as defined in swCenterMarkConnectionLine\_e

*LinearSlotCenter*
:   True to add center marks to slot centers, false to add them to slot ends

*ArcSlotCenter*
:   True to add center marks to arc centers, false to add them to arc ends

*UseDocumentDefaults*
:   True to use the display settings specified in **Tools > Options > Document Properties > Centerlines/Center Marks**, false to use the display settings set by this method

*Size*
:   Size of center mark; valid only if UseDocumentDefaults is false

*Gap*
:   Size of gap between the center mark and extension line; valid only if UseDocumentDefaults is false and the**Tools > Options > Document Properties > Centerlines/Center Marks > Scale by view scale** check box is clear (see **Remarks**)

*ExtendedLines*
:   True to extend lines from center mark points, false to not; valid only if UseDocumentDefaults is false

*CenterLineFont*
:   True to use the centerline font, false to not; valid only if UseDocumentDefaults is false

*Angle*
:   Rotation angle for the center mark; a positive angle rotates the center mark counterclockwise

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::AutoInsertCenterMarks2.

# ![](dotnetimages/collapse.gif)Example

[Automatically Insert Center Marks (C#)](Auto_Insert_Center_Marks_Example_CSharp.htm)

[Automatically Insert Center Marks (VB.NET)](Auto_Insert_Center_Marks_Example_VBNET.htm)

[Automatically Insert Center Marks (VBA)](Auto_Insert_Center_Marks_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method on each active view in which you want to insert center marks.

Before calling this method:

1. Call [IDrawingDoc::ActivateView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~ActivateView.html) with the name of the view to activate.- Call [IDrawingDoc::ActiveDrawingView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~ActiveDrawingView.html) to get a handle on the activated view.

Call [IDrawingDoc::InsertCenterMark3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~InsertCenterMark3.html) if you want to insert one center mark in one view.

| To... | Call... |
| --- | --- |
| Get the **Tools > Options > Document Properties > Centerlines/Center Marks > Scale by view scale** setting | [IModelDocExtension::GetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetUserPreferenceToggle.html) swUserPreferenceToggle\_e.swDetailingCenterMarkScaleByViewScale, swUserPreferenceOption\_e.swDetailingNoOptionSpecified |
| Set the **Tools > Options > Document Properties > Centerlines/Center Marks > Scale by view scale** setting | [IModelDocExtension::SetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetUserPreferenceToggle.html) swUserPreferenceToggle\_e.swDetailingCenterMarkScaleByViewScale, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, <*value*> |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetCenterMarkCount2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetCenterMarkCount2.html)

[IView::GetCenterMarkInfo Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetCenterMarkInfo.html)

[IView::GetCenterMarks Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetCenterMarks.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0