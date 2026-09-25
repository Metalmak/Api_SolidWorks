<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetReferenceCoordinateSystem2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetReferenceCoordinateSystem2 Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetReferenceCoordinateSystem2 Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BGlobal*
:   -1 or true to use the global coordinate system, 0 or false to use the coordinate system specified by DispRefEntity

*DispRefEntity*
:   User-defined coordinate system; valid only if BGlobal = false

Sets the coordinate system used for interpreting the location and direction of the remote load, mass, or displacement.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetReferenceCoordinateSystem2( _    ByVal BGlobal As System.Boolean, _    ByVal DispRefEntity As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BGlobal As System.Boolean Dim DispRefEntity As System.Object   instance.SetReferenceCoordinateSystem2(BGlobal, DispRefEntity) ``` | |

| C# |  |
| --- | --- |
| ``` void SetReferenceCoordinateSystem2(     System.bool BGlobal,    System.object DispRefEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetReferenceCoordinateSystem2(  &   System.bool BGlobal, &   System.Object^ DispRefEntity ) ``` | |

#### Parameters

*BGlobal*
:   -1 or true to use the global coordinate system, 0 or false to use the coordinate system specified by DispRefEntity

*DispRefEntity*
:   User-defined coordinate system; valid only if BGlobal = false

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30