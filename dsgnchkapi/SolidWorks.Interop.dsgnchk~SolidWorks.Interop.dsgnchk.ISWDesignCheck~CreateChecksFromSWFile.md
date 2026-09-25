<!-- source: dsgnchkapi/SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~CreateChecksFromSWFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Design Checker API Help | Send comments on this topic. |
| CreateChecksFromSWFile Method (ISWDesignCheck) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html) > [ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html) : CreateChecksFromSWFile Method (ISWDesignCheck) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*bstrSWFileName*
:   Full path name of an existing SOLIDWORKS document or template (**see Remarks**)

Creates checks in the Check Builder Module from an existing SOLIDWORKS document, template, or drafting standard.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateChecksFromSWFile( _    ByVal bstrSWFileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWDesignCheck Dim bstrSWFileName As System.String Dim value As System.Integer   value = instance.CreateChecksFromSWFile(bstrSWFileName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateChecksFromSWFile(     System.string bstrSWFileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateChecksFromSWFile(  &   System.String^ bstrSWFileName ) ``` | |

#### Parameters

*bstrSWFileName*
:   Full path name of an existing SOLIDWORKS document or template (**see Remarks**)

#### Return Value

Error code as defined in [dsgnchkError\_e](SOLIDWORKS.Interop.dsgnchk~SOLIDWORKS.Interop.dsgnchk.dsgnchkError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWDesignCheck::CreateChecksFromSWFile.

# ![](dotnetimages/collapse.gif)Example

[Create Checks From Document Example (VBA)](Create_Checks_From_Document_Example_VB.htm)

[Create Checks From Document Example (VB.NET)](Create_Checks_From_Document_Example_VBNET.htm)

[Create Checks From Document Example (C#)](Create_Checks_From_Document_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method can build checks from any of the following types of document:

* DWG (\*.dwg), * Part (\*.prt,\*.sldprt)* Assembly (\*.asm,\*.sldasm)* Drawing (\*.drw,\*.slddrw)* Template (\*.prtdot,\*.asmdot,\*.drwdot)* Drafting Standard (\*.sldstd)

# ![](dotnetimages/collapse.gif)See Also

####

[ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html)

[ISWDesignCheck Members](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck_members.html)

[ISWDesignCheck::CheckAgainstExistingFile Method](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~CheckAgainstExistingFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0