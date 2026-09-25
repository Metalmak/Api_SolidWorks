<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~ReloadTemplate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReloadTemplate Method (ISheet) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html) : ReloadTemplate Method (ISheet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*KeepNoteChanges*
:   True to keep note modifications made to the sheet format and reload all other elements from the original sheet format template, false to reload all elements from the original sheet format template and discard any note modifications made to the sheet format

Reloads the sheet format from the original sheet format template.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReloadTemplate( _    ByVal KeepNoteChanges As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISheet Dim KeepNoteChanges As System.Boolean Dim value As System.Integer   value = instance.ReloadTemplate(KeepNoteChanges) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ReloadTemplate(     System.bool KeepNoteChanges ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ReloadTemplate(  &   System.bool KeepNoteChanges ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*KeepNoteChanges*
:   True to keep note modifications made to the sheet format and reload all other elements from the original sheet format template, false to reload all elements from the original sheet format template and discard any note modifications made to the sheet format

#### Return Value

Status as defined in swReloadTemplateResult\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sheet::ReloadTemplate.

# ![](dotnetimages/collapse.gif)Example

[Modify and Reload Sheet Format Template (C#)](Modify_and_Reload_Sheet_Format_Template_Example_CSharp.htm)

[Modify and Reload Sheet Format Template (VB.NET)](Modify_and_Reload_Sheet_Format_Template_Example_VBNET.htm)

[Modify and Reload Sheet Format Template (VBA)](Modify_and_Reload_Sheet_Format_Template_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If new notes are added or existing notes modified or deleted on the sheet format, then specifying true for KeepNoteChanges:

* adds the new notes to the sheet format template, but does not duplicate the new notes on the sheet format.* restores any deleted notes from the sheet format template on the sheet format.* duplicates all other notes in their original position from the sheet format template on the sheet format.

# ![](dotnetimages/collapse.gif)See Also

####

[ISheet Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet.html)

[ISheet Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet_members.html)

[IDrawingDoc::EditTemplate Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~EditTemplate.html)

[ISheet::SaveFormat Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISheet~SaveFormat.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0