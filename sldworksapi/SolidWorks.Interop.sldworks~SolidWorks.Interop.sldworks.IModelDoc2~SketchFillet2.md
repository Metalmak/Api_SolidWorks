<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchFillet2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchFillet2 Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchFillet2 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Rad*
:   Radius of the fillet in meters

*ConstrainedCorners*
:   Action to take if the corner to be filleted is constrained or has a dimension  (see **Remarks**)

Obsolete. Superseded by [ISketchManager::CreateFillet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~CreateFillet.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchFillet2( _    ByVal Rad As System.Double, _    ByVal ConstrainedCorners As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Rad As System.Double Dim ConstrainedCorners As System.Short Dim value As System.Boolean   value = instance.SketchFillet2(Rad, ConstrainedCorners) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchFillet2(     System.double Rad,    System.short ConstrainedCorners ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchFillet2(  &   System.double Rad, &   System.short ConstrainedCorners ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Rad*
:   Radius of the fillet in meters

*ConstrainedCorners*
:   Action to take if the corner to be filleted is constrained or has a dimension  (see **Remarks**)

#### Return Value

True if the fillet is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchFillet2.

# ![](dotnetimages/collapse.gif)Remarks

The ConstrainedCorners argument:

* Indicates what action to take if the corner to be filleted is constrained in some manner or has a dimension related to it. In this case, adding a fillet to the corner cannot be done without certain consequences. If the corner is not involved with any constraints, this argument is ignored.

  * Can take one of the values found in swConstrainedCornerAction\_e.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0