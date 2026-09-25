<!-- source: dsgnchkapi/SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~CheckAgainstExistingFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Design Checker API Help | Send comments on this topic. |
| CheckAgainstExistingFile Method (ISWDesignCheck) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html) > [ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html) : CheckAgainstExistingFile Method (ISWDesignCheck) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Validates an active document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub CheckAgainstExistingFile() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWDesignCheck   instance.CheckAgainstExistingFile() ``` | |

| C# |  |
| --- | --- |
| ``` void CheckAgainstExistingFile() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CheckAgainstExistingFile(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWDesignCheck::CheckAgainstExistingFile.

# ![](dotnetimages/collapse.gif)Example

[Check Against Existing File Example (VBA)](Check_Against_Existing_File_Example_VB.htm)

[Check Against Existing File Example (VB.NET)](Check_Against_Existing_File_Example_VBNET.htm)

[Check Against Existing File Example (C#)](Check_Against_Existing_File_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method launches a dialog from which to choose a file. After the file is selected, Check Builder launches and creates checks from it. After the checks are built, Design Checker validates the active document against the checks and displays the results on a tab in the SOLIDWORKS Task Pane.

# ![](dotnetimages/collapse.gif)See Also

####

[ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html)

[ISWDesignCheck Members](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck_members.html)

[ISWDesignCheck::CreateChecksFromSWFile Method](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~CreateChecksFromSWFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0