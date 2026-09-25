<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~AddDynamicClearance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddDynamicClearance Method (IDragOperator) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDragOperator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator.html) : AddDynamicClearance Method (IDragOperator) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Comp1*
:   First component of the clearance pair

*Comp2*
:   Second component of the clearance pair

*Value*
:   Minimum clearance distance

*AppendFlag*
:   True appends the component to the list, false overwrites the list

*ShowDim*
:   True displays a dynamic reference dimension of the minimum clearance distance

Adds a dynamic clearance detector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDynamicClearance( _    ByVal Comp1 As System.Object, _    ByVal Comp2 As System.Object, _    ByVal Value As System.Double, _    ByVal AppendFlag As System.Boolean, _    ByVal ShowDim As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDragOperator Dim Comp1 As System.Object Dim Comp2 As System.Object Dim Value As System.Double Dim AppendFlag As System.Boolean Dim ShowDim As System.Boolean Dim value As System.Integer   value = instance.AddDynamicClearance(Comp1, Comp2, Value, AppendFlag, ShowDim) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddDynamicClearance(     System.object Comp1,    System.object Comp2,    System.double Value,    System.bool AppendFlag,    System.bool ShowDim ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddDynamicClearance(  &   System.Object^ Comp1, &   System.Object^ Comp2, &   System.double Value, &   System.bool AppendFlag, &   System.bool ShowDim ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Comp1*
:   First component of the clearance pair

*Comp2*
:   Second component of the clearance pair

*Value*
:   Minimum clearance distance

*AppendFlag*
:   True appends the component to the list, false overwrites the list

*ShowDim*
:   True displays a dynamic reference dimension of the minimum clearance distance

#### Return Value

Newly added clearance pair

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DragOperator::AddDynamicClearance.

# ![](dotnetimages/collapse.gif)See Also

####

[IDragOperator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator.html)

[IDragOperator Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator_members.html)

[IDragOperator::IAddDynamicClearance Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~IAddDynamicClearance.html)

[IDragOperator::DynamicClearanceEnabled Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDragOperator~DynamicClearanceEnabled.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0