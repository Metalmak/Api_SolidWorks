<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetBentLeaderLength.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBentLeaderLength Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetBentLeaderLength Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UseDoc*
:   True to use the document default setting for dimension bent leader, false to use the length argument for the bent leader length

*Length*
:   Length of the bent leader in system units

Sets the bent leader length to use for this dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBentLeaderLength( _    ByVal UseDoc As System.Boolean, _    ByVal Length As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim UseDoc As System.Boolean Dim Length As System.Double Dim value As System.Boolean   value = instance.SetBentLeaderLength(UseDoc, Length) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetBentLeaderLength(     System.bool UseDoc,    System.double Length ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetBentLeaderLength(  &   System.bool UseDoc, &   System.double Length ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UseDoc*
:   True to use the document default setting for dimension bent leader, false to use the length argument for the bent leader length

*Length*
:   Length of the bent leader in system units

#### Return Value

True if the bent leader length is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetBentLeaderLength.

# ![](dotnetimages/collapse.gif)Remarks

The dimension bent leader length only applies to these types of dimensions: radial and linear. If this method is used on any other type of dimension, no action is taken, and the return value is false.

Use:

* [IDisplayDimension::GetUseDocBentLeaderLength](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetUseDocBentLeaderLength.html) to determine whether this dimension is using the document default setting for dimension bent leader length or not.

  * [IDisplayDimension::GetBentLeaderLength](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetBentLeaderLength.html) to determine the bent leader length for this dimension.

After using this method, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window to see your changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)