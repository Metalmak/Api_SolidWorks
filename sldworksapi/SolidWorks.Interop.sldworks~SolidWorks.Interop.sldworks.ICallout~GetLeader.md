<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~GetLeader.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetLeader Method (ICallout) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html) : GetLeader Method (ICallout) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Visible*
:   True if leader is displayed, false if not (see **Remarks**)

*Multiple*
:   True if multiple leaders are displayed, false if not

Gets the leader properties of the callout.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetLeader( _    ByRef Visible As System.Boolean, _    ByRef Multiple As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICallout Dim Visible As System.Boolean Dim Multiple As System.Boolean Dim value As System.Boolean   value = instance.GetLeader(Visible, Multiple) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetLeader(     out System.bool Visible,    out System.bool Multiple ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetLeader(  &   [Out] System.bool Visible, &   [Out] System.bool Multiple ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Visible*
:   True if leader is displayed, false if not (see **Remarks**)

*Multiple*
:   True if multiple leaders are displayed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Callout::GetLeader.

# ![](dotnetimages/collapse.gif)Remarks

If Visible is false, then [ICallout::TargetStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout~TargetStyle.html) is swCalloutTargetStyle\_None.

# ![](dotnetimages/collapse.gif)See Also

####

[ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html)

[ICallout Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout_members.html)

[ICallout::SetLeader Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~SetLeader.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0