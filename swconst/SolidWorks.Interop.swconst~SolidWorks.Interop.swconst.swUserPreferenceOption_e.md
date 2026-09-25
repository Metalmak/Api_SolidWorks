<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceOption_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swUserPreferenceOption\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swUserPreferenceOption\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

User-preference enumerators for customizing document-level annotation, dimension, table, and view-label drafting standards.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swUserPreferenceOption_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swUserPreferenceOption_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swUserPreferenceOption_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swUserPreferenceOption_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDetailingAngleDimension** | See System Options and Document Properties. |
| **swDetailingAngularRunningDimension** | See System Options and Document Properties. |
| **swDetailingAnnotation** | See System Options and Document Properties. |
| **swDetailingArcLengthDimension** | See System Options and Document Properties. |
| **swDetailingAuxiliaryView** | See System Options and Document Properties. |
| **swDetailingBalloon** | See System Options and Document Properties. |
| **swDetailingBendTable** | See System Options and Document Properties. |
| **swDetailingBillOfMaterial** | See System Options and Document Properties. |
| **swDetailingChamferDimension** | See System Options and Document Properties. |
| **swDetailingDatum** | See System Options and Document Properties. |
| **swDetailingDetailView** | See System Options and Document Properties. |
| **swDetailingDiameterDimension** | See System Options and Document Properties. |
| **swDetailingDimension** | See System Options and Document Properties. |
| **swDetailingDrawingView** | See System Options and Document Properties. |
| **swDetailingGeneralTable** | See System Options and Document Properties. |
| **swDetailingGeometricTolerance** | See System Options and Document Properties. |
| **swDetailingHoleDimension** | See System Options and Document Properties. |
| **swDetailingHoleTable** | See System Options and Document Properties. |
| **swDetailingLinearDimension** | See System Options and Document Properties. |
| **swDetailingLocationLabel** | See System Options and Document Properties. |
| **swDetailingMiscView** | See System Options and Document Properties. |
| **swDetailingNoOptionSpecified** | See System Options and Document Properties. |
| **swDetailingNote** | See System Options and Document Properties. |
| **swDetailingOrdinateDimension** | See System Options and Document Properties. |
| **swDetailingOrthoView** | See System Options and Document Properties. |
| **swDetailingPunchTable** | See System Options and Document Properties. |
| **swDetailingRadiusDimension** | See System Options and Document Properties. |
| **swDetailingRevisionCloud** | See System Options and Document Properties. |
| **swDetailingRevisionTable** | See System Options and Document Properties. |
| **swDetailingSectionView** | See System Options and Document Properties. |
| **swDetailingSurfaceFinishSymbol** | See System Options and Document Properties. |
| **swDetailingTableAnnotation** | See System Options and Document Properties. |
| **swDetailingWeldSymbol** | See System Options and Document Properties. |
| **swDetailingWeldTable** | See System Options and Document Properties. |

# ![](dotnetimages/collapse.gif)Remarks

Use with:

* IModelDocExtension::GetUserPreferenceDouble and IModelDocExtension::SetUserPreferenceDouble* IModelDocExtension::GetUserPreferenceInteger and IModelDocExtension::SetUserPreferenceInteger * IModelDocExtension::GetUserPreferenceString and IModelDocExtension::SetUserPreferenceString * IModelDocExtension::GetUserPreferenceTextFormat and IModelDocExtension::SetUserPreferenceTextFormat* IModelDocExtension::GetUserPreferenceToggle and IModelDocExtension::SetUserPreferenceToggle

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)