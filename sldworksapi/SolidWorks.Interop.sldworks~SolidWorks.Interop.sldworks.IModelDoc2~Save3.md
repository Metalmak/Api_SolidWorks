<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~Save3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Save3 Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : Save3 Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Options*
:   Mode in which to save the document as defined in swSaveAsOptions\_e

*Errors*
:   Errors that caused the save operation to fail as defined in swFileSaveError\_e

*Warnings*
:   Warnings or extra information generated during the save operation as defined in swFileSaveWarning\_e

Saves the current document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Save3( _    ByVal Options As System.Integer, _    ByRef Errors As System.Integer, _    ByRef Warnings As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Options As System.Integer Dim Errors As System.Integer Dim Warnings As System.Integer Dim value As System.Boolean   value = instance.Save3(Options, Errors, Warnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Save3(     System.int Options,    out System.int Errors,    out System.int Warnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Save3(  &   System.int Options, &   [Out] System.int Errors, &   [Out] System.int Warnings ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*
:   Mode in which to save the document as defined in swSaveAsOptions\_e

*Errors*
:   Errors that caused the save operation to fail as defined in swFileSaveError\_e

*Warnings*
:   Warnings or extra information generated during the save operation as defined in swFileSaveWarning\_e

#### Return Value

True if the save was successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::Save3.

# ![](dotnetimages/collapse.gif)Example

[Save File (VBA)](Save_File_Example_VB.htm)

[Save File (VB.NET)](Save_File_Example_VBNET.htm)

[Save File (C#)](Save_File_Example_CSharp.htm)

[Rename Component and Update References (C#)](Rename_Component_and_Update_References_Example_CSharp.htm)

[Rename Component and Update References (VB.NET)](Rename_Component_and_Update_References_Example_VBNET.htm)

[Rename Component and Update References (VBA)](Rename_Component_and_Update_References_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| **If saving the file...** | **Then...** |
| --- | --- |
| Succeeds | * Return value is true * Errors argument is 0 |
| Fails | * Return value is false * Errors argument contains a bitwise OR of the error codes that were generated when saving the document |

You can find the masks to check against in the swFileSaveError\_e enumeration.

Even if the file is saved successfully, there might be warnings or information that occur during the save that might interest you. The Warnings argument contains a bitwise OR of the warning codes that were generated when saving the document. You can find the masks to check against in the swFileSaveWarning\_e enumeration.

| **If you do not want SOLIDWORKS to return...** | **Then pass in null or Nothing for...** |
| --- | --- |
| Error information | Errors argument |
| Warning information | Warnings argument |

This method results in FileSaveNotify being sent to any application listening.

See [IModelDocExtension::SaveAs](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SaveAs.html) if this is new document, this document is to be saved to a file with a new name, or this document is to be saved to a version of a particular format.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[ISldWorks::QuitDoc Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~QuitDoc.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0