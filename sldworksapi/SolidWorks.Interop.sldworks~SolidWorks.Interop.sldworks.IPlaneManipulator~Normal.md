<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPlaneManipulator~Normal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Normal Property (IPlaneManipulator) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPlaneManipulator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPlaneManipulator.html) : Normal Property (IPlaneManipulator) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the normal-to vector for a plane that has a manipulator.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Normal As MathVector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPlaneManipulator Dim value As MathVector   instance.Normal = value   value = instance.Normal ``` | |

| C# |  |
| --- | --- |
| ``` MathVector Normal {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property MathVector^ Normal {    MathVector^ get();    void set ( &   MathVector^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

[Normal-to vector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PlaneManipulator::Normal.

# ![](dotnetimages/collapse.gif)Remarks

If a plane with a manipulator is already displayed, then do not set a new normal-to vector or [origin](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPlaneManipulator~Origin.html) for that plane.

# ![](dotnetimages/collapse.gif)See Also

####

[IPlaneManipulator Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPlaneManipulator.html)

[IPlaneManipulator Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPlaneManipulator_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0