<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument~CompareDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| CompareDocument Method (ICompareDocument) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [ICompareDocument Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument.html) : CompareDocument Method (ICompareDocument) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*reffile*

*modfile*

*lOperationOptions*

*lResultOptions*

*reportname*

Obsolete. Superseded by [ICompareDocument::CompareDocument2](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.ICompareDocument~CompareDocument2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CompareDocument( _    ByVal reffile As System.String, _    ByVal modfile As System.String, _    ByVal lOperationOptions As System.Integer, _    ByVal lResultOptions As System.Integer, _    ByVal reportname As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICompareDocument Dim reffile As System.String Dim modfile As System.String Dim lOperationOptions As System.Integer Dim lResultOptions As System.Integer Dim reportname As System.String Dim value As System.Integer   value = instance.CompareDocument(reffile, modfile, lOperationOptions, lResultOptions, reportname) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CompareDocument(     System.string reffile,    System.string modfile,    System.int lOperationOptions,    System.int lResultOptions,    System.string reportname ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CompareDocument(  &   System.String^ reffile, &   System.String^ modfile, &   System.int lOperationOptions, &   System.int lResultOptions, &   System.String^ reportname ) ``` | |

#### Parameters

*reffile*

*modfile*

*lOperationOptions*

*lResultOptions*

*reportname*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ICompareDocument::CompareDocument.

# ![](dotnetimages/collapse.gif)See Also

####

[ICompareDocument Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument.html)

[ICompareDocument Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument_members.html)