<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration3~GetImportedBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetImportedBody Method (ISwDMConfiguration3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration3 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration3.html) : GetImportedBody Method (ISwDMConfiguration3) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*index*
:   Number indicating which imported solid body in this configuration to get

*fileName*
:   File to which to write the body in Parasolid .x\_b format (see Remarks)

Gets the imported solid body in this configuration and writes the body to the specified file in Parasolid .x\_b format.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetImportedBody( _    ByVal index As System.Integer, _    ByVal fileName As System.String _ ) As SwDmBodyError ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration3 Dim index As System.Integer Dim fileName As System.String Dim value As SwDmBodyError   value = instance.GetImportedBody(index, fileName) ``` | |

| C# |  |
| --- | --- |
| ``` SwDmBodyError GetImportedBody(     System.int index,    System.string fileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SwDmBodyError GetImportedBody(  &   System.int index, &   System.String^ fileName ) ``` | |

#### Parameters

*index*
:   Number indicating which imported solid body in this configuration to get

*fileName*
:   File to which to write the body in Parasolid .x\_b format (see Remarks)

#### Return Value

Success or error code as defined by [SwDmBodyError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmBodyError.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration3::GetImportedBody.

# ![](dotnetimages/collapse.gif)Remarks

This method gets imported solid bodies only; it does not get imported surface bodies.

Before calling this method, call [ISwConfiguration3::GetImportedBodiesCount](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMConfiguration3~GetImportedBodiesCount.html) to get the number of imported solid bodies in the configuration.

|  |  |
| --- | --- |
| **If fileName...** | **Then this method...** |
| Exists | Writes the imported solid body to fileName in Parasolid .x\_b format, overwriting any data in that file |
| Does not exist | Creates fileName and writes the imported solid body to that file in Parasolid .x\_b format |

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration3 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration3.html)

[ISwDMConfiguration3 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2004 SP2