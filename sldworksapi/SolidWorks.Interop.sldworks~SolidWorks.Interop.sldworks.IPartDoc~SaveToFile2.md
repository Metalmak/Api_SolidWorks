<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~SaveToFile2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveToFile2 Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : SaveToFile2 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Name of the part document (.sldprt)

*Options*
:   Relevant options indicating how to save the document as defined in swSaveAsOptions\_e

*Errors*
:   Errors that caused the save to fail as defined in swFileSaveError\_e

*Warnings*
:   Warnings or extra information generated during the save operation as defined in swFileSaveWarning\_e

Obsolete. Superseded by [IPartDoc::SaveToFile3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPartDoc~SaveToFile3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveToFile2( _    ByVal Name As System.String, _    ByVal Options As System.Integer, _    ByRef Errors As System.Integer, _    ByRef Warnings As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Name As System.String Dim Options As System.Integer Dim Errors As System.Integer Dim Warnings As System.Integer Dim value As System.Boolean   value = instance.SaveToFile2(Name, Options, Errors, Warnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveToFile2(     System.string Name,    System.int Options,    out System.int Errors,    out System.int Warnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveToFile2(  &   System.String^ Name, &   System.int Options, &   [Out] System.int Errors, &   [Out] System.int Warnings ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Name of the part document (.sldprt)

*Options*
:   Relevant options indicating how to save the document as defined in swSaveAsOptions\_e

*Errors*
:   Errors that caused the save to fail as defined in swFileSaveError\_e

*Warnings*
:   Warnings or extra information generated during the save operation as defined in swFileSaveWarning\_e

#### Return Value

True if the save is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::SaveToFile2.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP2, Revision Number 12.2