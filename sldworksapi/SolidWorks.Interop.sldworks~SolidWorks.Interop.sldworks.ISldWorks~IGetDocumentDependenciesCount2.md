<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IGetDocumentDependenciesCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetDocumentDependenciesCount2 Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : IGetDocumentDependenciesCount2 Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Document*
:   Name of the document

*Traverseflag*
:   True if you want to traverse down into all dependent files, false if you want only the highest level within the dependencies

*Searchflag*
:   Set this argument to True if you want to use the search rules to find dependencies, false looks where the documents were last saved

*AddReadOnlyInfo*
:   True if you want to have read-only information with the filenames, false if not

Gets the size of the array needed for a call to [ISldWorks::IGetDocumetnDependencies2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~IGetDocumentDependencies2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetDocumentDependenciesCount2( _    ByVal Document As System.String, _    ByVal Traverseflag As System.Boolean, _    ByVal Searchflag As System.Boolean, _    ByVal AddReadOnlyInfo As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Document As System.String Dim Traverseflag As System.Boolean Dim Searchflag As System.Boolean Dim AddReadOnlyInfo As System.Boolean Dim value As System.Integer   value = instance.IGetDocumentDependenciesCount2(Document, Traverseflag, Searchflag, AddReadOnlyInfo) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetDocumentDependenciesCount2(     System.string Document,    System.bool Traverseflag,    System.bool Searchflag,    System.bool AddReadOnlyInfo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetDocumentDependenciesCount2(  &   System.String^ Document, &   System.bool Traverseflag, &   System.bool Searchflag, &   System.bool AddReadOnlyInfo ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Document*
:   Name of the document

*Traverseflag*
:   True if you want to traverse down into all dependent files, false if you want only the highest level within the dependencies

*Searchflag*
:   Set this argument to True if you want to use the search rules to find dependencies, false looks where the documents were last saved

*AddReadOnlyInfo*
:   True if you want to have read-only information with the filenames, false if not

#### Return Value

Number of strings returned by [ISldWorks::IGetDocumetnDependencies2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~IGetDocumentDependencies2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::IGetDocumentDependenciesCount2.

# ![](dotnetimages/collapse.gif)Remarks

If SearchFlag is set to True, then the current directory is set to the directory of the document file. This is the same as interactively clikcing the References button in the File Open dialog.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetDocumentDependencies2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDocumentDependencies2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0