<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~GetVectorVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetVectorVB Method (IParameter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html) : GetVectorVB Method (IParameter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Extracts information of type vector from a parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetVectorVB() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParameter Dim value As System.Object   value = instance.GetVectorVB() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetVectorVB() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetVectorVB(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of 3 values in the vector (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Parameter::GetVectorVB.

# ![](dotnetimages/collapse.gif)Remarks

This method packs the data into a SafeArray in Visual Basic for Applications (VBA):

[ X,Y,Z ]

where:

|  |  |
| --- | --- |
| (double) X | x vector value stored on the parameter |
| (double) Y | y vector value stored on the parameter |
| (double) Z | z vector value stored on the parameter |

# ![](dotnetimages/collapse.gif)See Also

####

[IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html)

[IParameter Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter_members.html)

[IParameter::GetVector Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~GetVector.html)

[IParameter::SetVector2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~SetVector2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1998319