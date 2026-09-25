<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker~GetMessageIDs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| GetMessageIDs Method (ISwAddinAdvancedOptionBroker) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwAddinAdvancedOptionBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker.html) : GetMessageIDs Method (ISwAddinAdvancedOptionBroker) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IDs*
:   Array of dismissed message IDs

*Message*
:   Array of dismissed message strings

Gets all of the dismissed messages currently listed on **Tools > Options > System Options > Messages/Errors/Warnings**.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetMessageIDs( _    ByRef IDs As System.Object, _    ByRef Message As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddinAdvancedOptionBroker Dim IDs As System.Object Dim Message As System.Object   instance.GetMessageIDs(IDs, Message) ``` | |

| C# |  |
| --- | --- |
| ``` void GetMessageIDs(     out System.object IDs,    out System.object Message ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetMessageIDs(  &   [Out] System.Object^ IDs, &   [Out] System.Object^ Message ) ``` | |

#### Parameters

*IDs*
:   Array of dismissed message IDs

*Message*
:   Array of dismissed message strings

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddinAdvancedOptionBroker::GetMessageIDs.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddinAdvancedOptionBroker Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker.html)

[ISwAddinAdvancedOptionBroker Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker_members.html)

[ISwAddinAdvancedOptionBroker::SetMessageIDs Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddinAdvancedOptionBroker~SetMessageIDs.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0