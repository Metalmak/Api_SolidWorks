<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass~IGetCoordinates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetCoordinates Method (ICenterOfMass) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICenterOfMass Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass.html) : IGetCoordinates Method (ICenterOfMass) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the coordinates of this center of mass.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetCoordinates() As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICenterOfMass Dim value As System.Double   value = instance.IGetCoordinates() ``` | |

| C# |  |
| --- | --- |
| ``` System.double IGetCoordinates() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double IGetCoordinates(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

* in-process, unmanaged C++: Pointer to an array of doubles of the x, y, and z coordinates of the center of mass

  * VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICenterOfMass Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass.html)

[ICenterOfMass Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass_members.html)

[ICenterOfMass::GetCoordinates Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass~GetCoordinates.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0