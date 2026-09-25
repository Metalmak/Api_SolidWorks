<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICalloutVariable~ShowParenthesis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ShowParenthesis Property (ICalloutVariable) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICalloutVariable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICalloutVariable.html) : ShowParenthesis Property (ICalloutVariable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to show parentheses around linear tolerance dimensions in a hole callout.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ShowParenthesis As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICalloutVariable Dim value As System.Boolean   instance.ShowParenthesis = value   value = instance.ShowParenthesis ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowParenthesis {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ShowParenthesis {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to show parentheses around linear tolerance dimensions, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CalloutVariable::ShowParenthesis.

# ![](dotnetimages/collapse.gif)Remarks

This property supports bilateral, symmetric, or fit-with-tolerance types only.

In SOLIDWORKS 2016 and later, use this property to set whether to show parentheses around linear tolerance dimensions in a hole callout. Calling [IDimensionTolerance::ShowParenthesis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionTolerance~ShowParenthesis.html) to set whether to show parentheses around linear tolerance dimensions in a hole callout does not override this property's setting.

# ![](dotnetimages/collapse.gif)See Also

####

[ICalloutVariable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICalloutVariable.html)

[ICalloutVariable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICalloutVariable_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0