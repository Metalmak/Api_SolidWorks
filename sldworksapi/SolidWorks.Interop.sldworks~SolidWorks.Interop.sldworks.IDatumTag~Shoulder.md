<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTag~Shoulder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Shoulder Property (IDatumTag) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDatumTag Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTag.html) : Shoulder Property (IDatumTag) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether there is a shoulder (or bend) in the leader for this datum tag.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Shoulder As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDatumTag Dim value As System.Boolean   instance.Shoulder = value   value = instance.Shoulder ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Shoulder {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool Shoulder {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True if this datum tag has a shoulder, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DatumTag::Shoulder.

# ![](dotnetimages/collapse.gif)Remarks

Although you get or set this property at any time, this property only applies to square datum tags. If you use it when a round datum tag is shown, you will not see a value for the current display.

# ![](dotnetimages/collapse.gif)See Also

####

[IDatumTag Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTag.html)

[IDatumTag Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTag_members.html)

[IDatumTag::ForcedShoulder Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTag~ForcedShoulder.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0