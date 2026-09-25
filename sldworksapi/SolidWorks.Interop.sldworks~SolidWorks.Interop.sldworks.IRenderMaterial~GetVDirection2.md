<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~GetVDirection2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetVDirection2 Method (IRenderMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html) : GetVDirection2 Method (IRenderMaterial) |

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

Gets the V direction of the texture-based appearance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetVDirection2( _    ByRef VDir_X As System.Double, _    ByRef VDir_Y As System.Double, _    ByRef VDir_Z As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRenderMaterial Dim VDir_X As System.Double Dim VDir_Y As System.Double Dim VDir_Z As System.Double   instance.GetVDirection2(VDir_X, VDir_Y, VDir_Z) ``` | |

| C# |  |
| --- | --- |
| ``` void GetVDirection2(     out System.double VDir_X,    out System.double VDir_Y,    out System.double VDir_Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetVDirection2(  &   [Out] System.double VDir_X, &   [Out] System.double VDir_Y, &   [Out] System.double VDir_Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VDir\_X*
:   X coordinate of the V direction

*VDir\_Y*
:   Y coordinate of the V direction

*VDir\_Z*
:   Z coordinate of the V direction

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenderMaterial::GetVDirection2.

# ![](dotnetimages/collapse.gif)Example

See [IRenderMaterial](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The [mapping type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial~MappingType.html) (surface, projection, automatic, etc.) indirectly determines the V direction. This vector is perpendicular to the U direction.

Call [IRenderMaterial::GetUDirection2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial~GetUDirection2.html) to get the U direction of the appearance.

# ![](dotnetimages/collapse.gif)See Also

####

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

[IRenderMaterial Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial_members.html)

[IRenderMaterial::SetUDirection2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~SetUDirection2.html)

[IRenderMaterial::SetVDirection2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial~SetVDirection2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 SP05, Revision 21.5