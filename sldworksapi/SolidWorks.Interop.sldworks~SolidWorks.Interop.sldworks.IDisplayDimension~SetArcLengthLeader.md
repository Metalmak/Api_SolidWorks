<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetArcLengthLeader.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetArcLengthLeader Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetArcLengthLeader Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AutoLeader*
:   True if the leader style is automatically selected, false if the leader style is
    selected by the user

*LeaderType*
:   Leader style as defined in swArcLengthLeaderType\_e if autoLeader is false

Sets the leader style of this arc-length dimension.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetArcLengthLeader( _    ByVal AutoLeader As System.Boolean, _    ByVal LeaderType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim AutoLeader As System.Boolean Dim LeaderType As System.Integer Dim value As System.Integer   value = instance.SetArcLengthLeader(AutoLeader, LeaderType) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetArcLengthLeader(     System.bool AutoLeader,    System.int LeaderType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetArcLengthLeader(  &   System.bool AutoLeader, &   System.int LeaderType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AutoLeader*
:   True if the leader style is automatically selected, false if the leader style is
    selected by the user

*LeaderType*
:   Leader style as defined in swArcLengthLeaderType\_e if autoLeader is false

#### Return Value

Return status:

|  |  |
| --- | --- |
| 0 | Command was successful, leader style values were set |
| -1 | Command failed for an unknown reason, no leader style values were set |
| -2 | Specified leader style value is not valid |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetArcLengthLeader.

# ![](dotnetimages/collapse.gif)Remarks

The leader style of an arc length dimension is specific to each display dimension. The leader style can be parallel (the leaders are parallel to each other) or radial (the leaders are perpendicular to the extension line and would extend through the center of the arc). The style can be selected automatically by SOLIDWORKS, or specified by the user.

If the autoLeader value is passed in as True to automatically select the leader style, then SOLIDWORKS ignores the leaderStyle value.

This method applies only to arc length dimensions. It does not affect any other types of dimensions.

After using this method, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window to see your changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

[IDisplayDimensioin::GetArcLengthLeader Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~GetArcLengthLeader.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207