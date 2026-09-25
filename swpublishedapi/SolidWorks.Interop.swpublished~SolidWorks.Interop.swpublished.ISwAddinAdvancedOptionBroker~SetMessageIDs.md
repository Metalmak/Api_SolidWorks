<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker~SetMessageIDs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| SetMessageIDs Method (ISwAddinAdvancedOptionBroker) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwAddinAdvancedOptionBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker.html) : SetMessageIDs Method (ISwAddinAdvancedOptionBroker) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IDs*
:   Array of IDs of dismissed messages to display (see **Remarks**)

Sets the specified dismissed messages to display on **Tools > Options > System Options > Messages/Errors/Warnings**.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMessageIDs( _    ByVal IDs As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddinAdvancedOptionBroker Dim IDs As System.Object   instance.SetMessageIDs(IDs) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMessageIDs(     System.object IDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMessageIDs(  &   System.Object^ IDs ) ``` | |

#### Parameters

*IDs*
:   Array of IDs of dismissed messages to display (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddinAdvancedOptionBroker::SetMessageIDs.

# ![](dotnetimages/collapse.gif)Remarks

By omission, this method effectively removes one or more dismissed messages from the list on **Tools > Options > System Options > Messages/Errors/Warnings**.

Before calling this method use [ISwAddinAdvancedOptionBroker::GetMessageIDs](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwAddinAdvancedOptionBroker~GetMessageIDs.html) to obtain the IDs of the current list of dismissed messages.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddinAdvancedOptionBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker.html)

[ISwAddinAdvancedOptionBroker Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0