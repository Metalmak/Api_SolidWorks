<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~SetCenterPoint2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetCenterPoint2 Method (IRenderMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html) : SetCenterPoint2 Method (IRenderMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CenterPt\_X*
:   X coordinate of the center point

*CenterPt\_Y*
:   Y coordinate of the center point

*CenterPt\_Z*
:   Z coordinate of the center point

Sets the center point of the mapping for texture-based appearances.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetCenterPoint2( _    ByVal CenterPt_X As System.Double, _    ByVal CenterPt_Y As System.Double, _    ByVal CenterPt_Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRenderMaterial Dim CenterPt_X As System.Double Dim CenterPt_Y As System.Double Dim CenterPt_Z As System.Double   instance.SetCenterPoint2(CenterPt_X, CenterPt_Y, CenterPt_Z) ``` | |

| C# |  |
| --- | --- |
| ``` void SetCenterPoint2(     System.double CenterPt_X,    System.double CenterPt_Y,    System.double CenterPt_Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetCenterPoint2(  &   System.double CenterPt_X, &   System.double CenterPt_Y, &   System.double CenterPt_Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CenterPt\_X*
:   X coordinate of the center point

*CenterPt\_Y*
:   Y coordinate of the center point

*CenterPt\_Z*
:   Z coordinate of the center point

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenderMaterial::SetCenterPoint2.

# ![](dotnetimages/collapse.gif)Remarks

This method is required to properly position a texture-based appearance (e.g., if you need a specific corner of a face to have the black square of a checkered-pattern appearance).

# ![](dotnetimages/collapse.gif)See Also

####

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

[IRenderMaterial Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial_members.html)

[IRenderMaterial::GetCenterPoint2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~GetCenterPoint2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP05, Revision 21.5