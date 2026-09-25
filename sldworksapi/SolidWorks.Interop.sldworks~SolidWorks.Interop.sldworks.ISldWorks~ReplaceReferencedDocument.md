<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ReplaceReferencedDocument.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplaceReferencedDocument Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : ReplaceReferencedDocument Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReferencingDocument*
:   Document whose references to modify; the document cannot be open

*ReferencedDocument*
:   Document is referenced by ReferencingDocument; all of its references within ReferencingDocument are replaced by NewReference

*NewReference*
:   New document used by ReferencingDocument

Replaces a referenced document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceReferencedDocument( _    ByVal ReferencingDocument As System.String, _    ByVal ReferencedDocument As System.String, _    ByVal NewReference As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim ReferencingDocument As System.String Dim ReferencedDocument As System.String Dim NewReference As System.String Dim value As System.Boolean   value = instance.ReplaceReferencedDocument(ReferencingDocument, ReferencedDocument, NewReference) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplaceReferencedDocument(     System.string ReferencingDocument,    System.string ReferencedDocument,    System.string NewReference ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplaceReferencedDocument(  &   System.String^ ReferencingDocument, &   System.String^ ReferencedDocument, &   System.String^ NewReference ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReferencingDocument*
:   Document whose references to modify; the document cannot be open

*ReferencedDocument*
:   Document is referenced by ReferencingDocument; all of its references within ReferencingDocument are replaced by NewReference

*NewReference*
:   New document used by ReferencingDocument

#### Return Value

True if the the referenced document is replaced, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::ReplaceReferencedDocument.

# ![](dotnetimages/collapse.gif)Example

[Replace Referenced Document (VBA)](Replace_Referenced_Document_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Mates, dimensions, and other references might fail when the referencingDocument is opened.

If the internal ID of the ReferencedDocument does not match the internal ID of the NewReference document, then an error message is displayed when the ReferencingDocument is opened. The internal ID is a time stamp that was generated when the file was created. Unless the NewReference is actually a renamed copy of the ReferencedDocument document, then it is unlikely that the internal IDs will match.

This method does not check for the existence of the NewReference document. If the document does not exist when the ReferencingDocument is opened, then the user is warned and prompted to browse for a replacement.

The ReferencedDocument and NewReference file types must match. For example, if ReferencingDocument is an assembly with four subassemblies, you cannot replace any of the subassembly references with a part document. If you were to replace any of the subassembly references, they would need to be replaced by another SOLIDWORKS assembly document.

You might also notice that the component name, which is visible in the FeatureManager design tree, will not change to the name of the NewReference unless the proper user preference is set (Tools, Options, System Options, External References, Update component names when documents are replaced).

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)