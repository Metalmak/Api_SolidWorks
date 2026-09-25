<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetDocumentSaveToNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDocumentSaveToNames Method (IPackAndGo) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html) : GetDocumentSaveToNames Method (IPackAndGo) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PathNameList*
:   Array of strings containing the path and filenames to which to save the model's documents (see **Remarks**)

*DocumentStatusList*
:   Array containing the types of documents as defined in swPackAndGoDocumentStatus\_e

Gets the paths and filenames to which to save the model's documents for Pack and Go set by [IPackAndGo::SetDocumentSaveToNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~SetDocumentSaveToNames.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDocumentSaveToNames( _    ByRef PathNameList As System.Object, _    ByRef DocumentStatusList As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPackAndGo Dim PathNameList As System.Object Dim DocumentStatusList As System.Object Dim value As System.Boolean   value = instance.GetDocumentSaveToNames(PathNameList, DocumentStatusList) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetDocumentSaveToNames(     out System.object PathNameList,    out System.object DocumentStatusList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetDocumentSaveToNames(  &   [Out] System.Object^ PathNameList, &   [Out] System.Object^ DocumentStatusList ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PathNameList*
:   Array of strings containing the path and filenames to which to save the model's documents (see **Remarks**)

*DocumentStatusList*
:   Array containing the types of documents as defined in swPackAndGoDocumentStatus\_e

#### Return Value

True if the paths and filenames of the model's documents are returned, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PackAndGo::GetDocumentSaveToNames.

# ![](dotnetimages/collapse.gif)Example

[Pack and Go an Assembly (C#)](Pack_and_Go_an_Assembly_Example_CSharp.htm)

[Pack and Go an Assembly (VB.NET)](Pack_and_Go_an_Assembly_Example_VBNET.htm)

[Pack and Go an Assembly (VBA)](Pack_and_Go_an_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The order and number of documents must match the order of the array returned by [IPackAndGo::GetDocumentNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~GetDocumentNames.html). If a [prefix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~AddPrefix.html) or [suffix](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~AddSuffix.html) is set, then the filenames include it. You can set both a prefix and suffix for the filenames.

# ![](dotnetimages/collapse.gif)See Also

####

[IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html)

[IPackAndGo Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo_members.html)

[IPackAndGo::IGetDocumentSaveToNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IGetDocumentSaveToNames.html)

[IPackAndGo::ISetDocumentSaveToNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~ISetDocumentSaveToNames.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0