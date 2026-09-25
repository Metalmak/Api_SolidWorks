<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetMirrorOrientation2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMirrorOrientation2 Method (ICWCompositeShellOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html) : SetMirrorOrientation2 Method (ICWCompositeShellOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Face to which material orientation is applied

*BMirrorOri*
:   0 or false for clockwise ply angle direction, -1 or true for counter-clockwise ply angle direction

Sets the ply angle mirror orientation of this composite shell.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetMirrorOrientation2( _    ByVal DispEntity As System.Object, _    ByVal BMirrorOri As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWCompositeShellOptions Dim DispEntity As System.Object Dim BMirrorOri As System.Boolean Dim value As System.Integer   value = instance.SetMirrorOrientation2(DispEntity, BMirrorOri) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetMirrorOrientation2(     System.object DispEntity,    System.bool BMirrorOri ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetMirrorOrientation2(  &   System.Object^ DispEntity, &   System.bool BMirrorOri ) ``` | |

#### Parameters

*DispEntity*
:   Face to which material orientation is applied

*BMirrorOri*
:   0 or false for clockwise ply angle direction, -1 or true for counter-clockwise ply angle direction

#### Return Value

Error code as defined in [swsCompositeShellOptionsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCompositeShellOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWCompositeShellOptions::MappingType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~MappingType.html) is set to [swsCompositeShellOptionsMappingType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCompositeShellOptionsMappingType_e.html).swsCompositeShellOptionsSurfaceMapping.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html)

[ICWCompositeShellOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30