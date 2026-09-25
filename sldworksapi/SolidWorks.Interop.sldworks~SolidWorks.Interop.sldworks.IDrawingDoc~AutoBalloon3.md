<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~AutoBalloon3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutoBalloon3 Method (IDrawingDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : AutoBalloon3 Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Layout*
:   Layout style of the balloons as defined by swBalloonLayoutType\_e or specify -1 for this argument to use the document default layout style

*IgnoreMultiple*
:   True to apply a balloon to only one instance of a component, false to apply balloons to all instances of that component

*Style*
:   Style of the balloons as defined by swBalloonStyle\_e or specify -1 to use the document default balloon style

*Size*
:   Fit of balloon as defined by swBalloonFit\_e or specify -1 to use the document default balloon fit

*UpperTextContent*
:   Upper-text content style as defined by swBalloonTextContent\_e or specify -1 to use the document default upper text content

*UpperText*
:   Text for upper balloon

*LowerTextContent*
:   Lower-text content style as defined by swBalloonTextContent\_e or specify -1 to use the document default lower text content

    **NOTE:** This and the next argument are only effective when Style is set to swBS\_SplitCirc. See the SOLIDWORKS Help for additional details about autoballoons.

*LowerText*
:   Text for lower balloon

*Layername*
:   Name of the layer for this balloon

Obsolete. Superseded by [IDrawingDoc::AutoBalloon4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrawingDoc~AutoBalloon4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AutoBalloon3( _    ByVal Layout As System.Integer, _    ByVal IgnoreMultiple As System.Boolean, _    ByVal Style As System.Integer, _    ByVal Size As System.Integer, _    ByVal UpperTextContent As System.Integer, _    ByVal UpperText As System.String, _    ByVal LowerTextContent As System.Integer, _    ByVal LowerText As System.String, _    ByVal Layername As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc Dim Layout As System.Integer Dim IgnoreMultiple As System.Boolean Dim Style As System.Integer Dim Size As System.Integer Dim UpperTextContent As System.Integer Dim UpperText As System.String Dim LowerTextContent As System.Integer Dim LowerText As System.String Dim Layername As System.String Dim value As System.Object   value = instance.AutoBalloon3(Layout, IgnoreMultiple, Style, Size, UpperTextContent, UpperText, LowerTextContent, LowerText, Layername) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AutoBalloon3(     System.int Layout,    System.bool IgnoreMultiple,    System.int Style,    System.int Size,    System.int UpperTextContent,    System.string UpperText,    System.int LowerTextContent,    System.string LowerText,    System.string Layername ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AutoBalloon3(  &   System.int Layout, &   System.bool IgnoreMultiple, &   System.int Style, &   System.int Size, &   System.int UpperTextContent, &   System.String^ UpperText, &   System.int LowerTextContent, &   System.String^ LowerText, &   System.String^ Layername ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Layout*
:   Layout style of the balloons as defined by swBalloonLayoutType\_e or specify -1 for this argument to use the document default layout style

*IgnoreMultiple*
:   True to apply a balloon to only one instance of a component, false to apply balloons to all instances of that component

*Style*
:   Style of the balloons as defined by swBalloonStyle\_e or specify -1 to use the document default balloon style

*Size*
:   Fit of balloon as defined by swBalloonFit\_e or specify -1 to use the document default balloon fit

*UpperTextContent*
:   Upper-text content style as defined by swBalloonTextContent\_e or specify -1 to use the document default upper text content

*UpperText*
:   Text for upper balloon

*LowerTextContent*
:   Lower-text content style as defined by swBalloonTextContent\_e or specify -1 to use the document default lower text content

    **NOTE:** This and the next argument are only effective when Style is set to swBS\_SplitCirc. See the SOLIDWORKS Help for additional details about autoballoons.

*LowerText*
:   Text for lower balloon

*Layername*
:   Name of the layer for this balloon

#### Return Value

Array of newly created [notes](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::AutoBalloon3.

# ![](dotnetimages/collapse.gif)Example

[Insert AutoBalloons (VBA)](Insert_AutoBalloons_Example_VB_AutoBallooon3_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method automatically creates the BOM balloons for the selected drawing views. If a drawing sheet is selected, BOM balloons are automatically created for all of the drawing views on that drawing sheet.

|  |  |
| --- | --- |
| To get or set default values for... | Use... |
| Layout | [IModelDocExtension::GetUserPreferenceInteger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetUserPreferenceInteger.html)(swUserPreferenceIntegerValue\_e.swDetailingAutoBalloonLayout, swUserPreferenceOption\_e.swDetailingNoOptionSpecified)  - or - [IModelDocExtension::SetUserPreferenceInteger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SetUserPreferenceInteger.html)(swUserPreferenceIntegerValue\_e.swDetailingAutoBalloonLayout, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swBalloonLayoutType\_e.<Value>) |
| Style | IModelDocExtension::GetUserPreferenceInteger((swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonStyle, swUserPreferenceOption\_e.swDetailingNoOptionSpecified) - or - IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonFit, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swBalloonFit\_e.<Value>) |
| Size | IModelDocExtension::GetUserPreferenceInteger((swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonFit, swUserPreferenceOption\_e.swDetailingNoOptionSpecified) - or - (swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonFit, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swBalloonFit\_e.<Value>) |
| UpperTextContent | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMUpperText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified) -  or - IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMUpperText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swBalloonTextContent\_e.<Value>) |
| LowerTextContent | IModelDocExtension::GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMLowerText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified) - or - IModelDocExtension::SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMLowerText, swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swBalloonTextContent\_e.<Value>) |

This method also allows you to get only the balloons just created.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[IModelDocExtension::InsertBOMBalloon Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertBOMBalloon.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0