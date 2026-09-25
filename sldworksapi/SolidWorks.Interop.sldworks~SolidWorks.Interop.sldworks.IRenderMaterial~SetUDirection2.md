<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~SetUDirection2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUDirection2 Method (IRenderMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html) : SetUDirection2 Method (IRenderMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UDir\_X*
:   X coordinate of the U direction

*UDir\_Y*
:   Y coordinate of the U direction

*UDir\_Z*
:   Z coordinate of the U direction

Sets the U direction of the texture-based appearance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetUDirection2( _    ByVal UDir_X As System.Double, _    ByVal UDir_Y As System.Double, _    ByVal UDir_Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRenderMaterial Dim UDir_X As System.Double Dim UDir_Y As System.Double Dim UDir_Z As System.Double   instance.SetUDirection2(UDir_X, UDir_Y, UDir_Z) ``` | |

| C# |  |
| --- | --- |
| ``` void SetUDirection2(     System.double UDir_X,    System.double UDir_Y,    System.double UDir_Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetUDirection2(  &   System.double UDir_X, &   System.double UDir_Y, &   System.double UDir_Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UDir\_X*
:   X coordinate of the U direction

*UDir\_Y*
:   Y coordinate of the U direction

*UDir\_Z*
:   Z coordinate of the U direction

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenderMaterial::SetUDirection2.

# ![](dotnetimages/collapse.gif)Remarks

To specify the U direction in the X direction, set:

1. UDir\_X to 1.0.

   - UDir\_Y to 0.0.

     - UDir\_Z to 0.0.

Call [IRenderMaterial::SetVDirection2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial~SetVDirection2.html) to set the V direction of the appearance.

# ![](dotnetimages/collapse.gif)See Also

####

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

[IRenderMaterial Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial_members.html)

[IRenderMaterial::GetUDirection2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~GetUDirection2.html)

[IRenderMaterial::GetVDirection2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~GetVDirection2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP05, Revision 21.5