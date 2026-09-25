<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetOverride.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetOverride Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetOverride Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Override*
:   True to display a value other than the actual dimension value, false to display the actual value

*Value*
:   Value to display instead of the actual dimension value

Sets whether to display the actual dimension value or to display another value, and, if so, that value.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetOverride( _    ByVal Override As System.Boolean, _    ByVal Value As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim Override As System.Boolean Dim Value As System.Double Dim value As System.Boolean   value = instance.SetOverride(Override, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetOverride(     System.bool Override,    System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetOverride(  &   System.bool Override, &   System.double Value ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Override*
:   True to display a value other than the actual dimension value, false to display the actual value

*Value*
:   Value to display instead of the actual dimension value

#### Return Value

True if setting an override value is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetOverride.

# ![](dotnetimages/collapse.gif)Remarks

This method can only be used on a display dimension in a drawing. In a part or assembly, this method takes no action and returns false.

If Override is set to false, then the Value argument is ignored.

Use [IDisplayDimension::GetOverride](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetOverride.html) to get whether the actual dimension value or another value is displayed.

Use [IDisplayDimension::GetOverrideValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension~GetOverrideValue.html) to get the value to display instead of the actual dimension value.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)