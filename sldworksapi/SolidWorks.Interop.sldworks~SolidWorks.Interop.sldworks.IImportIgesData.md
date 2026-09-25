<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportIgesData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IImportIgesData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportIgesData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IImportIgesData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows you to specify levels and values when importing IGES data.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IImportIgesData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IImportIgesData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IImportIgesData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IImportIgesData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ImportIgesData.

# ![](dotnetimages/collapse.gif)Example

[Specify IGES Levels and Values, Then Import IGES File (C#)](Specify_IGES_Levels_and_Values_Then_Import_IGES_File_Example_CSharp.htm)

[Specify IGES Levels and Values, Then Import IGES File (VB.NET)](Specify_IGES_Levels_and_Values_Then_Import_IGES_File_Example_VBNET.htm)

[Specify IGES Levels and Values, Then Import IGES File (VBA)](Specify_IGES_Levels_and_Values%2C_Then_Import_IGES_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If user preference** **swIGESImportShowLevel** **is...** | **Then the IGES translator...** |
| True | Displays the IGES-In Surfaces, Curves, and Levels dialog to the user where the user can specify levels and values. |
| false and you retrieved IImportIgesData | Does not display the IGES-In Surfaces, Curves, and Levels dialog to the user and allows you to specify the levels and values. |
| false and you did not retrieve IImportIgesData | Does not display the IGES-In Surfaces, Curves, and Levels dialog to the user and uses the default values. |

To specify levels and values when importing IGES data:

> 1. Set the user preference swIGESImportShowLevel to false.
>
> 2. Use [ISldWorks::GetImportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetImportFileData.html) to get IImportIgesData.
>
> 3. Use the IImportIgesData functions to specify the levels and values.
>
> 4. Use [ISldworks::LoadFile4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~LoadFile4.html) to load the file.

# ![](dotnetimages/collapse.gif)Accessors

[ISldWorks::GetImportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetImportFileData.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[ImportIgesData](SWObjectModel.pdf#ImportIgesData)

# ![](dotnetimages/collapse.gif)See Also

####

[IImportIgesData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportIgesData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IImportDxfDwgData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImportDxfDwgData.html)