<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~InsertRadiateSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertRadiateSurface Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : InsertRadiateSurface Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Distance*
:   Distance to extend the surface

*FlipDir*
:   True to flip the direction; by default the direction is out from the center of the face

*TangentPropagate*
:   True to propagate the surface along tangent faces, false limits the surface to the selected face

Creates a radiate surface based on the selections.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertRadiateSurface( _    ByVal Distance As System.Double, _    ByVal FlipDir As System.Boolean, _    ByVal TangentPropagate As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Distance As System.Double Dim FlipDir As System.Boolean Dim TangentPropagate As System.Boolean   instance.InsertRadiateSurface(Distance, FlipDir, TangentPropagate) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertRadiateSurface(     System.double Distance,    System.bool FlipDir,    System.bool TangentPropagate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertRadiateSurface(  &   System.double Distance, &   System.bool FlipDir, &   System.bool TangentPropagate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Distance*
:   Distance to extend the surface

*FlipDir*
:   True to flip the direction; by default the direction is out from the center of the face

*TangentPropagate*
:   True to propagate the surface along tangent faces, false limits the surface to the selected face

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::InsertRadiateSurface.

# ![](dotnetimages/collapse.gif)Example

[Create Radiate Surface Feature (VBA)](Get_Radiate_Surface_Data_Example_VB.htm)

[Create Radiate Surface Feature (VB.NET)](Create_Radiate_Surface_Example_VBNET.htm)

[Create Radiate Surface Feature (C#)](Create_Radiate_Surface_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select

* Reference direction using Mark = 1.* Radiate entities using Mark = 2.

See the SOLIDWORKS Help for information about what entities are valid for selection.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[ISurfaceRadiateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceRadiateFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0