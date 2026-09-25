<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass~GetCoordinates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetCoordinates Method (ICenterOfMass) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICenterOfMass Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass.html) : GetCoordinates Method (ICenterOfMass) |

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
| ``` Function GetCoordinates() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICenterOfMass Dim value As System.Object   value = instance.GetCoordinates() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetCoordinates() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetCoordinates(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of doubles of the x, y, and z coordinates of the center of mass

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CenterOfMass::GetCoordinates.

# ![](dotnetimages/collapse.gif)Example

[Get Centers of Mass in Drawing Views (VBA)](Get_Centers_of_Mass_in_Drawing_Views_Example_VB.htm)

[Get Centers of Mass in Drawing Views (VB.NET)](Get_Centers_of_Mass_in_Drawing_Views_Example_VBNET.htm)

[Get Centers of Mass in Drawing Views (C#)](Get_Centers_of_Mass_in_Drawing_Views_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICenterOfMass Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass.html)

[ICenterOfMass Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass_members.html)

[ICenterOfMass::IGetCoordinates Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterOfMass~IGetCoordinates.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0