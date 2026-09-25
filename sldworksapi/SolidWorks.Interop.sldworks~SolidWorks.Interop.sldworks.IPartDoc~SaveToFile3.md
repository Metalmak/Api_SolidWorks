<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~SaveToFile3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SaveToFile3 Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : SaveToFile3 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Path and name of the part document to which to save the selected weldment member, solid body, or surface body

*Options*
:   How to save the document as defined in swSaveAsOptions\_e

*CutListProps*
:   Option for transferring the cut list of the selected weldment member, solid body, or surface body to the new part as defined in swCutListTransferOptions\_e

*OverrideTemplate*
:   True to override the part template with the template specified by TemplatePath, false to not

*TemplatePath*
:   Path to part template; valid only if OverrideTemplate is true

*Errors*
:   Save errors as defined in swFileSaveError\_e

*Warnings*
:   Warnings or extra information generated during the save operation as defined in swFileSaveWarning\_e

Saves the selected weldment member, surface body, or solid body to another part document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveToFile3( _    ByVal Name As System.String, _    ByVal Options As System.Integer, _    ByVal CutListProps As System.Integer, _    ByVal OverrideTemplate As System.Boolean, _    ByVal TemplatePath As System.String, _    ByRef Errors As System.Integer, _    ByRef Warnings As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim Name As System.String Dim Options As System.Integer Dim CutListProps As System.Integer Dim OverrideTemplate As System.Boolean Dim TemplatePath As System.String Dim Errors As System.Integer Dim Warnings As System.Integer Dim value As System.Boolean   value = instance.SaveToFile3(Name, Options, CutListProps, OverrideTemplate, TemplatePath, Errors, Warnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveToFile3(     System.string Name,    System.int Options,    System.int CutListProps,    System.bool OverrideTemplate,    System.string TemplatePath,    out System.int Errors,    out System.int Warnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveToFile3(  &   System.String^ Name, &   System.int Options, &   System.int CutListProps, &   System.bool OverrideTemplate, &   System.String^ TemplatePath, &   [Out] System.int Errors, &   [Out] System.int Warnings ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Path and name of the part document to which to save the selected weldment member, solid body, or surface body

*Options*
:   How to save the document as defined in swSaveAsOptions\_e

*CutListProps*
:   Option for transferring the cut list of the selected weldment member, solid body, or surface body to the new part as defined in swCutListTransferOptions\_e

*OverrideTemplate*
:   True to override the part template with the template specified by TemplatePath, false to not

*TemplatePath*
:   Path to part template; valid only if OverrideTemplate is true

*Errors*
:   Save errors as defined in swFileSaveError\_e

*Warnings*
:   Warnings or extra information generated during the save operation as defined in swFileSaveWarning\_e

#### Return Value

True if the save is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::SaveToFile3.

# ![](dotnetimages/collapse.gif)Example

[Save Solid Body to File (VBA)](Save_Solid_Body_to_File_Example_VB.htm)

[Save Solid Body to File (VB.NET)](Save_Solid_Body_to_File_Example_VBNET.htm)

[Save Solid Body to File (C#)](Save_Solid_Body_to_File_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The difference between this method and the now obsolete IPartDoc::SaveToFile2 is that this method allows you to specify in CutListProps how the cut list properties of the selected weldment member of a weldment part are transferred to the saved part.

Before calling this method, select a weldment member, surface body, or solid body in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0