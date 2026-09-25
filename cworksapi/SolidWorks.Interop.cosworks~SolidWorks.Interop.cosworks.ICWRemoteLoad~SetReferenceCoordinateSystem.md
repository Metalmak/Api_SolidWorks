<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetReferenceCoordinateSystem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReferenceCoordinateSystem Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetReferenceCoordinateSystem Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BGlobal*
:   1 to use the global coordinate system, 0 to use the coordinate system specified by DispRefEntity

*DispRefEntity*
:   User-defined coordinate system; valid only if BGlobal = 0

Obsolete. Superseded by [ICWRemoteLoad::SetReferenceCoordinateSystem2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetReferenceCoordinateSystem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReferenceCoordinateSystem( _    ByVal BGlobal As System.Integer, _    ByVal DispRefEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BGlobal As System.Integer Dim DispRefEntity As System.Object   instance.SetReferenceCoordinateSystem(BGlobal, DispRefEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReferenceCoordinateSystem(     System.int BGlobal,    System.object DispRefEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReferenceCoordinateSystem(  &   System.int BGlobal, &   System.Object^ DispRefEntity ) ``` | |

#### Parameters

*BGlobal*
:   1 to use the global coordinate system, 0 to use the coordinate system specified by DispRefEntity

*DispRefEntity*
:   User-defined coordinate system; valid only if BGlobal = 0

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::SetReferenceCoordinateSystem.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0