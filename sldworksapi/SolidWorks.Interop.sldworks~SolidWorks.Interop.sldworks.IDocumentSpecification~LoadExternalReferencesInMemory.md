<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~LoadExternalReferencesInMemory.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LoadExternalReferencesInMemory Property (IDocumentSpecification) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDocumentSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html) : LoadExternalReferencesInMemory Property (IDocumentSpecification) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to load external references in memory when opening a document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LoadExternalReferencesInMemory As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDocumentSpecification Dim value As System.Boolean   instance.LoadExternalReferencesInMemory = value   value = instance.LoadExternalReferencesInMemory ``` | |

| C# |  |
| --- | --- |
| ``` System.bool LoadExternalReferencesInMemory {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool LoadExternalReferencesInMemory {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to load external references in memory, false (default) to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DocumentSpecification::LoadExternalReferencesInMemory.

# ![](dotnetimages/collapse.gif)Remarks

This property is:

* not valid for opening **3D**EXPERIENCE files using SOLIDWORKS Connected.

* valid only if swUserPreferenceIntegerValue\_e.swLoadExternalReferences is not set to swLoadExternalReferences\_e.swLoadExternalReferences\_None.

Note: The **System Options > External References > Load documents in memory only** user preference and swUserPreferenceToggle\_e.swExtRefLoadRefDocsInMemory are ignored when opening documents through the API because this method and [ISldWorks::OpenDoc6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~OpenDoc6.html) (swOpenDocOptions\_e.swOpenDocOptions\_LoadExternalReferencesInMemory) have sole control of reference loading.

# ![](dotnetimages/collapse.gif)See Also

####

[IDocumentSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html)

[IDocumentSpecification Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0