<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~SetVDirection2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetVDirection2 Method (IRenderMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html) : SetVDirection2 Method (IRenderMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VDir\_X*
:   X coordinate of the V direction

*VDir\_Y*
:   Y coordinate of the V direction

*VDir\_Z*
:   Z coordinate of the V direction

Sets the V direction of the texture-based appearance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetVDirection2( _    ByVal VDir_X As System.Double, _    ByVal VDir_Y As System.Double, _    ByVal VDir_Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRenderMaterial Dim VDir_X As System.Double Dim VDir_Y As System.Double Dim VDir_Z As System.Double   instance.SetVDirection2(VDir_X, VDir_Y, VDir_Z) ``` | |

| C# |  |
| --- | --- |
| ``` void SetVDirection2(     System.double VDir_X,    System.double VDir_Y,    System.double VDir_Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetVDirection2(  &   System.double VDir_X, &   System.double VDir_Y, &   System.double VDir_Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VDir\_X*
:   X coordinate of the V direction

*VDir\_Y*
:   Y coordinate of the V direction

*VDir\_Z*
:   Z coordinate of the V direction

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenderMaterial::SetVDirection2.

# ![](dotnetimages/collapse.gif)Remarks

To specify the V direction in the Y direction, set:

1. VDir\_X to 0.0.

   - VDir\_Y to 1.0.

     - VDir\_Z to 0.0.

The [mapping type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial~MappingType.html) (surface, projection, automatic, etc.) indirectly determines the V direction. This vector is perpendicular to the U direction.

Call [IRenderMaterial::SetUDirection2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial~SetUDirection2.html) to set the U direction.

# ![](dotnetimages/collapse.gif)See Also

####

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

[IRenderMaterial Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial_members.html)

[IRenderMaterial::GetUDirection2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~GetUDirection2.html)

[IRenderMaterial::GetVDirection2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~GetVDirection2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP05, Revision 21.5