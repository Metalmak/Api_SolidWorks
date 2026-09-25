<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IGetDocumentSaveToNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetDocumentSaveToNames Method (IPackAndGo) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html) : IGetDocumentSaveToNames Method (IPackAndGo) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NameCount*
:   Number of documents comprising the model

*NameList*
:   * in-process, unmanaged C++: Pointer to an array of strings containing the paths and filenames of the model's documents* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*StatusList*
:   Array containing the types of documents as defined in swPackAndGoDocumentStatus\_e

Gets the paths and filenames to which to save the model's documents for Pack and Go set by [IPackAndGo::ISetDocumentSaveToNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~ISetDocumentSaveToNames.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetDocumentSaveToNames( _    ByVal NameCount As System.Integer, _    ByRef NameList As System.String, _    ByRef StatusList As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPackAndGo Dim NameCount As System.Integer Dim NameList As System.String Dim StatusList As System.Integer Dim value As System.Boolean   value = instance.IGetDocumentSaveToNames(NameCount, NameList, StatusList) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IGetDocumentSaveToNames(     System.int NameCount,    out System.string NameList,    out System.int StatusList ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IGetDocumentSaveToNames(  &   System.int NameCount, &   [Out] System.String^ NameList, &   [Out] System.int StatusList ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NameCount*
:   Number of documents comprising the model

*NameList*
:   * in-process, unmanaged C++: Pointer to an array of strings containing the paths and filenames of the model's documents* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*StatusList*
:   Array containing the types of documents as defined in swPackAndGoDocumentStatus\_e

#### Return Value

True if the paths and filenames of the model's documents are returned, false if not

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IPackAndGo::GetDocumentNamesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~GetDocumentNamesCount.html) to get the value of NameCount.

# ![](dotnetimages/collapse.gif)See Also

####

[IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html)

[IPackAndGo Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo_members.html)

[IPackAndGo::ISetDocumentSaveToNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~ISetDocumentSaveToNames.html)

[IPackAndGo::GetDocumentSaveToNames Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetDocumentSaveToNames.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0