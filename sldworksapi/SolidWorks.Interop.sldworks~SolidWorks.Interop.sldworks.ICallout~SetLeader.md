<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~SetLeader.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLeader Method (ICallout) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html) : SetLeader Method (ICallout) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Visible*
:   True to display the leader, false to not (see **Remarks**)

*Multiple*
:   True to display multiple leaders, false to not

Sets the leader properties of the callout.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLeader( _    ByVal Visible As System.Boolean, _    ByVal Multiple As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICallout Dim Visible As System.Boolean Dim Multiple As System.Boolean Dim value As System.Boolean   value = instance.SetLeader(Visible, Multiple) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetLeader(     System.bool Visible,    System.bool Multiple ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetLeader(  &   System.bool Visible, &   System.bool Multiple ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Visible*
:   True to display the leader, false to not (see **Remarks**)

*Multiple*
:   True to display multiple leaders, false to not

#### Return Value

True if the operation is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Callout::SetLeader.

# ![](dotnetimages/collapse.gif)Example

[Create a Callout Independent of a Selection (C#)](Create_a_Callout_Independent_of_a_Selection_Example_CSharp.htm)

[Create a Callout Independent of a Selection (VB.NET)](Create_a_Callout_Independent_of_a_Selection_Example_VBNET.htm)

[Create a Callout Independent of a Selection (VBA)](Create_a_Callout_Independent_of_a_Selection_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You can only use this method before the callout is shown or while the callout is hidden.

If Visible is set to false, then [ICallout::TargetStyle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout~TargetStyle.html) is automatically set to swCalloutTargetStyle\_None.

# ![](dotnetimages/collapse.gif)See Also

####

[ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html)

[ICallout Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout_members.html)

[ICallout::GetLeader Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~GetLeader.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0