<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~IGetTessTriangles.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetTessTriangles Method (IComponent2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : IGetTessTriangles Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NoConversion*
:   True prohibits conversion to user units from system units, false does not

Gets the triangles that make up the shaded picture tessellation for this component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetTessTriangles( _    ByVal NoConversion As System.Boolean _ ) As System.Single ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim NoConversion As System.Boolean Dim value As System.Single   value = instance.IGetTessTriangles(NoConversion) ``` | |

| C# |  |
| --- | --- |
| ``` System.float IGetTessTriangles(     System.bool NoConversion ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.float IGetTessTriangles(  &   System.bool NoConversion ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NoConversion*
:   True prohibits conversion to user units from system units, false does not

#### Return Value

* in-process, unmanaged C++: Pointer to array of floats (see **Remarks**)

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Tessellation information is available only when the component is loaded as lightweight.

These triangles are intended for graphics display purposes and do not represent a
tessellation that could be used, for example, by a machining application. If you
need the type of accuracy associated with a machining product, we recommend that
you traverse the body faces and extract the topology and geometry data to create
your own faceting.

The format of the returned data is:

* float x, y, z - first point in meters* float x, y, z - second point in meters* float x, y, z - third point in meters

for the set of triangles for the component.

The total size of the data is **[** 9 x sizeof(*float)* x *(number of triangles)* **]**.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IComponent2::GetTessTriangles Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~GetTessTriangles.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0