<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swRenameDocumentError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swRenameDocumentError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swRenameDocumentError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Rename components errors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swRenameDocumentError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swRenameDocumentError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swRenameDocumentError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swRenameDocumentError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swRenameDocumentError\_ComponentNotResolved** | 5 = You must resolve the component before attempting to rename it |
| **swRenameDocumentError\_DocumentNameInUse** | 12 = You cannot rename the component to the specified name because a document with that name is open |
| **swRenameDocumentError\_DocumentNotSaved** | 15 = You cannot rename the document, and the document was not saved |
| **swRenameDocumentError\_FileAlreadyExists** | 8 = You cannot rename the component to the specified name because a file with that name exists on disk |
| **swRenameDocumentError\_InvalidCharactersInName** | 9 = You specified an invalid component name; the name is either too long or contains invalid characters |
| **swRenameDocumentError\_InvalidForDrawings** | 3 = You cannot rename drawing documents |
| **swRenameDocumentError\_InvalidSelection** | 2 = You must select a valid component; your selection is invalid for renaming |
| **swRenameDocumentError\_InvalidVirtualComponent** | 10 = You cannot rename virtual components |
| **swRenameDocumentError\_LightWeightComponent** | 6 = You cannot rename the child component whose parent component is lightweight |
| **swRenameDocumentError\_NameTooLong** | 11 = You cannot rename the component to the specified name because that name is too long |
| **swRenameDocumentError\_NoModelLoaded** | 4 = You cannot rename the component because a model is not loaded in memory |
| **swRenameDocumentError\_None** | 0 = Success |
| **swRenameDocumentError\_NotAllowedWithPDM** | 17 = You cannot rename the component because the SOLIDWORKS Professional PDM add-in is not loaded |
| **swRenameDocumentError\_PatternedComponent** | 19 = You cannot rename patterned components |
| **swRenameDocumentError\_PendingNameAlreadyInUse** | 13 = You cannot rename the component to the specified name because a document with the same name has been temporarily renamed but not yet saved |
| **swRenameDocumentError\_ReadOnlyDocument** | 14 = You cannot rename read-only documents or documents referenced by read-only documents |
| **swRenameDocumentError\_RoutingComponent** | 7 = You cannot rename routing components |
| **swRenameDocumentError\_ToolboxComponent** | 18 = You cannot rename Toolbox components |
| **swRenameDocumentError\_UnspecifiedInternalError** | 1 = You cannot rename the component due to an internal error |
| **swRenameDocumentError\_VirtualComponent** | 16 = You cannot rename virtual components |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)