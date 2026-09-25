<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings~GetOffsets.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| GetOffsets Method (IBalloonSettings) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IBalloonSettings Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings.html) : GetOffsets Method (IBalloonSettings) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Offset type as defined by [swiBalloonSettingsOffsetTypes\_e](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.swiBalloonSettingsOffsetTypes_e.html)

*IsVisible*
:   True to balloon the offset type in the document, false to just include it in the inspection report

*X\_Offset*
:   X offset for the default location of the balloons

*Y\_Offset*
:   Y offset for the default location of the balloons

Gets whether to balloon the specified offset type in the document and gets the current offsets for the specified offset type.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetOffsets( _    ByVal Type As System.Integer, _    ByRef IsVisible As System.Boolean, _    ByRef X_Offset As System.Double, _    ByRef Y_Offset As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBalloonSettings Dim Type As System.Integer Dim IsVisible As System.Boolean Dim X_Offset As System.Double Dim Y_Offset As System.Double Dim value As System.Boolean   value = instance.GetOffsets(Type, IsVisible, X_Offset, Y_Offset) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetOffsets(     System.int Type,    out System.bool IsVisible,    out System.double X_Offset,    out System.double Y_Offset ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetOffsets(  &   System.int Type, &   [Out] System.bool IsVisible, &   [Out] System.double X_Offset, &   [Out] System.double Y_Offset ) ``` | |

#### Parameters

*Type*
:   Offset type as defined by [swiBalloonSettingsOffsetTypes\_e](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.swiBalloonSettingsOffsetTypes_e.html)

*IsVisible*
:   True to balloon the offset type in the document, false to just include it in the inspection report

*X\_Offset*
:   X offset for the default location of the balloons

*Y\_Offset*
:   Y offset for the default location of the balloons

#### Return Value

True if offset settings successfully retrieved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See BalloonSettings methods.

# ![](dotnetimages/collapse.gif)Remarks

X\_Offset and Y\_Offset are from the upper left-hand corner of the attribute to the upper left-hand corner of the balloon. The offsets can be positive or negative numbers.

For more information, see the Ballooning Settings PropertyManager - Offsets section of the **SOLIDWORKS Inspection Add-in user-interface help > SOLIDWORKS Inspection > SOLIDWORKS Inspection Add-in > Getting Started > Balloons** topic.

# ![](dotnetimages/collapse.gif)See Also

####

[IBalloonSettings Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings.html)

[IBalloonSettings Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IBalloonSettings_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS