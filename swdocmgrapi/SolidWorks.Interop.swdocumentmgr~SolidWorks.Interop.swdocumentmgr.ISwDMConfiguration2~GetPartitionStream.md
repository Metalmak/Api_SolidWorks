<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration2~GetPartitionStream.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetPartitionStream Method (ISwDMConfiguration2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMConfiguration2 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration2.html) : GetPartitionStream Method (ISwDMConfiguration2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fileName*
:   Filename to which to write the Parasolid partition and body information (see Remarks)

Gets the Parasolid partition stream that has the body partition information and writes it the specified file. Supports part documents only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPartitionStream( _    ByVal fileName As System.String _ ) As SwDmBodyError ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMConfiguration2 Dim fileName As System.String Dim value As SwDmBodyError   value = instance.GetPartitionStream(fileName) ``` | |

| C# |  |
| --- | --- |
| ``` SwDmBodyError GetPartitionStream(     System.string fileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SwDmBodyError GetPartitionStream(  &   System.String^ fileName ) ``` | |

#### Parameters

*fileName*
:   Filename to which to write the Parasolid partition and body information (see Remarks)

#### Return Value

Success or error code as defined by [SwDmBodyError](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.SwDmBodyError.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMConfiguration2::GetPartitionStream.

# ![](dotnetimages/collapse.gif)Example

[Write Parasolid Partition Stream to File (C#)](Write_Parasolid_Partition_Stream_to_File_Example_CSharp.htm)

[Write Parasolid Partition Stream to File (VB.NET)](Write_Parasolid_Partition_Stream_to_File_Example_VBNET.htm)

[Write Parasolid Partition Stream to File (C++)](Write_Parasolid_Partition_Stream_to_File_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only supports part documents saved in SOLIDWORKS 2004 and later. Use [ISwDMConfiguration::GetBody](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMConfiguration~GetBody.html) for part dcouments saved in SOLIDWORKS 2003 and earlier and assembly documents saved in any version of SOLIDWORKS.

To get the version of a part document, use [ISwDMDocument::GetVersion](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMDocument~GetVersion.html).

Before using this method, call [ISwDMConfiguration2::PartitionStreamName](SOLIDWORKS.Interop.swdocumentmgr~SOLIDWORKS.Interop.swdocumentmgr.ISwDMConfiguration2~PartitionStreamName.html) to get fileName. Valid filename extensions are \*.xmp\_bin for NTFS and \*.p\_b for FAT.

|  |  |
| --- | --- |
| **If fileName...** | **Then...** |
| Does not exit | This method creates the file and writes the Parasolid partition and body information to that file |
| Exists | Writes the Parasolid partition and body information to that file, overwriting any data in that file |

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMConfiguration2 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration2.html)

[ISwDMConfiguration2 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMConfiguration2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2004 SP1