<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareFeature~CompareFeatures2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| CompareFeatures2 Method (ICompareFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [ICompareFeature Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareFeature.html) : CompareFeatures2 Method (ICompareFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*reffile*
:   Path and filename of the SOLIDWORKS document containing the referenced part

*refconfig*
:   Name of the reference part's configuration; if blank, then the active configuration is used

*modfile*
:   Path and filename of the SOLIDWORKS document containing the modified part

*modconfig*
:   Name of modified part's configuration

*lOptions*
:   Display the results or save the results to a report as defined by [gtResultOptions\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtResultOptions_e.html)

*reportname*
:   Path where to save the results report

*vtAddToBinderOption*
:   True to add the results report to the Design Binder, false to not

*vtOverwrite*
:   True to overwrite an existing results report of the same name, false to not

Identifies the differences in solid features between two versions of the same SOLIDWORKS part and generates a report.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CompareFeatures2( _    ByVal reffile As System.String, _    ByVal refconfig As System.String, _    ByVal modfile As System.String, _    ByVal modconfig As System.String, _    ByVal lOptions As System.Integer, _    ByVal reportname As System.String, _    ByVal vtAddToBinderOption As System.Boolean, _    ByVal vtOverwrite As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICompareFeature Dim reffile As System.String Dim refconfig As System.String Dim modfile As System.String Dim modconfig As System.String Dim lOptions As System.Integer Dim reportname As System.String Dim vtAddToBinderOption As System.Boolean Dim vtOverwrite As System.Boolean Dim value As System.Integer   value = instance.CompareFeatures2(reffile, refconfig, modfile, modconfig, lOptions, reportname, vtAddToBinderOption, vtOverwrite) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CompareFeatures2(     System.string reffile,    System.string refconfig,    System.string modfile,    System.string modconfig,    System.int lOptions,    System.string reportname,    System.bool vtAddToBinderOption,    System.bool vtOverwrite ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CompareFeatures2(  &   System.String^ reffile, &   System.String^ refconfig, &   System.String^ modfile, &   System.String^ modconfig, &   System.int lOptions, &   System.String^ reportname, &   System.bool vtAddToBinderOption, &   System.bool vtOverwrite ) ``` | |

#### Parameters

*reffile*
:   Path and filename of the SOLIDWORKS document containing the referenced part

*refconfig*
:   Name of the reference part's configuration; if blank, then the active configuration is used

*modfile*
:   Path and filename of the SOLIDWORKS document containing the modified part

*modconfig*
:   Name of modified part's configuration

*lOptions*
:   Display the results or save the results to a report as defined by [gtResultOptions\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtResultOptions_e.html)

*reportname*
:   Path where to save the results report

*vtAddToBinderOption*
:   True to add the results report to the Design Binder, false to not

*vtOverwrite*
:   True to overwrite an existing results report of the same name, false to not

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ICompareFeature::CompareFeatures2.

# ![](dotnetimages/collapse.gif)Example

[Compare Features (VBA)](Compare_Features_VB6.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICompareFeature Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareFeature.html)

[ICompareFeature Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2006 FCS