<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences~AddFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFile Method (IEdmUpdateReferences) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUpdateReferences Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences.html) : AddFile Method (IEdmUpdateReferences) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oPath*
:   Full path to the file for which to update file references

Adds an assembly or drawing to the batch of files for which to update file references.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFile( _    ByVal oPath As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFile(     System.object oPath ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFile(  &   System.Object^ oPath ) ``` | |

#### Parameters

*oPath*
:   Full path to the file for which to update file references

# ![](dotnetimages/collapse.gif)Example

[Update References (C#)](Update_References_Example_CSharp.htm)

[Update References (VB.NET)](Update_References_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUpdateReferences Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences.html)

[IEdmUpdateReferences Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011