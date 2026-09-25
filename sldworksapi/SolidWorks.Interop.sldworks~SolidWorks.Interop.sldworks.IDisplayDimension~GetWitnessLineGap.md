<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetWitnessLineGap.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetWitnessLineGap Method (IDisplayDimension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : GetWitnessLineGap Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WitnessIndex*
:   Index of the extension line whose gap to get

*UseDoc*
:   True if using the document default value of the gap, false if not (see **Remarks**)

*Gap*
:   Gap value in system units (see **Remarks**)

Gets the gap of the specified dimension extension line.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetWitnessLineGap( _    ByVal WitnessIndex As System.Short, _    ByRef UseDoc As System.Boolean, _    ByRef Gap As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim WitnessIndex As System.Short Dim UseDoc As System.Boolean Dim Gap As System.Double Dim value As System.Boolean   value = instance.GetWitnessLineGap(WitnessIndex, UseDoc, Gap) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetWitnessLineGap(     System.short WitnessIndex,    out System.bool UseDoc,    out System.double Gap ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetWitnessLineGap(  &   System.short WitnessIndex, &   [Out] System.bool UseDoc, &   [Out] System.double Gap ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WitnessIndex*
:   Index of the extension line whose gap to get

*UseDoc*
:   True if using the document default value of the gap, false if not (see **Remarks**)

*Gap*
:   Gap value in system units (see **Remarks**)

#### Return Value

True if the operation succeeds, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::GetWitnessLineGap.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Dimension Extension Lines Gap (VBA)](Get_and_Set_Dimension_Extension_Lines_Gaps_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The UseDoc argument is dependent on the detailing standard. You can retrieve the document default value using the document-level user-preference swDetailingWitnessLineGap.

The Gap argument is the document default value if UseDoc is true; otherwise, the value returned is the locally set value.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimension::SetWitnessLineGap Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetWitnessLineGap.html)

[IView::GetDimensionInfo6 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDimensionInfo6.html)

[IView::IGetDimensionInfo6 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetDimensionInfo6.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0