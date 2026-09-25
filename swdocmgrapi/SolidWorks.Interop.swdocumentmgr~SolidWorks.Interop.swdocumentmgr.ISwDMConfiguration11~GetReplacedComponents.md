<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11~GetReplacedComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetReplacedComponents Method (ISwDMConfiguration11) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration11 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11.html) : GetReplacedComponents Method (ISwDMConfiguration11) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentNames*
:   Array of component names that were replaced

*ConfigurationNames*
:   :   Array of configuration names for the components that were replaced in the document

*NewFilenames*
:   Array of the path and filenames of the components that were replaced

*MatesReattached*
:   :   Array of Booleans indicating whether the mates for the components that were replaced were reattached

Gets information about the components that were replaced by [ISwDMComponent6::Replace](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMComponent6~Replace.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetReplacedComponents( _    ByRef ComponentNames As System.Object, _    ByRef ConfigurationNames As System.Object, _    ByRef NewFilenames As System.Object, _    ByRef MatesReattached As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration11 Dim ComponentNames As System.Object Dim ConfigurationNames As System.Object Dim NewFilenames As System.Object Dim MatesReattached As System.Object   instance.GetReplacedComponents(ComponentNames, ConfigurationNames, NewFilenames, MatesReattached) ``` | |

| C# |  |
| --- | --- |
| ``` void GetReplacedComponents(     out System.object ComponentNames,    out System.object ConfigurationNames,    out System.object NewFilenames,    out System.object MatesReattached ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetReplacedComponents(  &   [Out] System.Object^ ComponentNames, &   [Out] System.Object^ ConfigurationNames, &   [Out] System.Object^ NewFilenames, &   [Out] System.Object^ MatesReattached ) ``` | |

#### Parameters

*ComponentNames*
:   Array of component names that were replaced

*ConfigurationNames*
:   :   Array of configuration names for the components that were replaced in the document

*NewFilenames*
:   Array of the path and filenames of the components that were replaced

*MatesReattached*
:   :   Array of Booleans indicating whether the mates for the components that were replaced were reattached

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration11::GetReplacedComponents.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration11 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11.html)

[ISwDMConfiguration11 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration11_members.html)

[ISwDMDocument8::GetChangedReferences Method](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument8~GetChangedReferences.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2009 SP0