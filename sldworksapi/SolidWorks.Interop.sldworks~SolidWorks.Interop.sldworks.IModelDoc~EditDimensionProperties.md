<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~EditDimensionProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditDimensionProperties Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : EditDimensionProperties Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TolType*

*TolMax*

*TolMin*

*TolMaxFit*

*TolMinFit*

*UseDocPrec*

*Precision*

*ArrowsIn*

*UseDocArrows*

*Arrow1*

*Arrow2*

Obsolete. Superseded by [IModelDoc2::EditDimensionProperties](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditDimensionProperties.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditDimensionProperties( _    ByVal TolType As System.Integer, _    ByVal TolMax As System.Double, _    ByVal TolMin As System.Double, _    ByVal TolMaxFit As System.String, _    ByVal TolMinFit As System.String, _    ByVal UseDocPrec As System.Boolean, _    ByVal Precision As System.Integer, _    ByVal ArrowsIn As System.Integer, _    ByVal UseDocArrows As System.Boolean, _    ByVal Arrow1 As System.Integer, _    ByVal Arrow2 As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim TolType As System.Integer Dim TolMax As System.Double Dim TolMin As System.Double Dim TolMaxFit As System.String Dim TolMinFit As System.String Dim UseDocPrec As System.Boolean Dim Precision As System.Integer Dim ArrowsIn As System.Integer Dim UseDocArrows As System.Boolean Dim Arrow1 As System.Integer Dim Arrow2 As System.Integer Dim value As System.Boolean   value = instance.EditDimensionProperties(TolType, TolMax, TolMin, TolMaxFit, TolMinFit, UseDocPrec, Precision, ArrowsIn, UseDocArrows, Arrow1, Arrow2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EditDimensionProperties(     System.int TolType,    System.double TolMax,    System.double TolMin,    System.string TolMaxFit,    System.string TolMinFit,    System.bool UseDocPrec,    System.int Precision,    System.int ArrowsIn,    System.bool UseDocArrows,    System.int Arrow1,    System.int Arrow2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool EditDimensionProperties(  &   System.int TolType, &   System.double TolMax, &   System.double TolMin, &   System.String^ TolMaxFit, &   System.String^ TolMinFit, &   System.bool UseDocPrec, &   System.int Precision, &   System.int ArrowsIn, &   System.bool UseDocArrows, &   System.int Arrow1, &   System.int Arrow2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TolType*

*TolMax*

*TolMin*

*TolMaxFit*

*TolMinFit*

*UseDocPrec*

*Precision*

*ArrowsIn*

*UseDocArrows*

*Arrow1*

*Arrow2*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::EditDimensionProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)