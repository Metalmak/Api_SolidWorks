<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetMenuStrings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetMenuStrings Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetMenuStrings Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CommandID*
:   Command ID of the command whose parent menu's name you want

*DocumentType*
:   Document types in which this command exists as defined in swDocumentTypes\_e

*ParentMenuName*
:   Name of the parent menu of the specified menu command

Gets the name of the parent menu of the specified menu command.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMenuStrings( _    ByVal CommandID As System.Integer, _    ByVal DocumentType As System.Integer, _    ByRef ParentMenuName As System.String _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim CommandID As System.Integer Dim DocumentType As System.Integer Dim ParentMenuName As System.String Dim value As System.String   value = instance.GetMenuStrings(CommandID, DocumentType, ParentMenuName) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetMenuStrings(     System.int CommandID,    System.int DocumentType,    out System.string ParentMenuName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetMenuStrings(  &   System.int CommandID, &   System.int DocumentType, &   [Out] System.String^ ParentMenuName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CommandID*
:   Command ID of the command whose parent menu's name you want

*DocumentType*
:   Document types in which this command exists as defined in swDocumentTypes\_e

*ParentMenuName*
:   Name of the parent menu of the specified menu command

#### Return Value

Menu string

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetMenuStrings.

# ![](dotnetimages/collapse.gif)Remarks

Use this method with methods that require you to supply the name of the menu, such as [ISldWorks::RemoveMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RemoveMenu.html), [IFrame::RenameMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFrame~RenameMenu.html) and [IFrame::RemoveMenu](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFrame~RemoveMenu.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP2, Revision Number 15.2