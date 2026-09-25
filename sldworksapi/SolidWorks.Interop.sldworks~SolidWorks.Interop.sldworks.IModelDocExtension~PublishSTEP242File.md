<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~PublishSTEP242File.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PublishSTEP242File Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : PublishSTEP242File Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Path*
:   Full qualified path to which to export the SOLIDWORKS MBD 3D part or assembly; use **.STP** for the file name extension

Exports the SOLIDWORKS MBD 3D part or assembly to a STEP 242 file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function PublishSTEP242File( _    ByVal Path As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Path As System.String Dim value As System.Integer   value = instance.PublishSTEP242File(Path) ``` | |

| C# |  |
| --- | --- |
| ``` System.int PublishSTEP242File(     System.string Path ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int PublishSTEP242File(  &   System.String^ Path ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Path*
:   Full qualified path to which to export the SOLIDWORKS MBD 3D part or assembly; use **.STP** for the file name extension

#### Return Value

Status as defined in swStep242Error\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::PublishSTEP242File.

# ![](dotnetimages/collapse.gif)Example

[Export SOLIDWORKS MBD to STEP 242 (C#)](Export_SOLIDWORKS_MBD_to_STEP_242_Example_CSharp.htm)

[Export SOLIDWORKS MBD to STEP 242 (VB.NET)](Export_SOLIDWORKS_MBD_to_STEP_242_Example_VBNET.htm)

[Export SOLIDWORKS MBD to STEP 242 (VBA)](Export_SOLIDWORKS_MBD_to_STEP_242_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::PublishTo3DPDF Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~PublishTo3DPDF.html)

[IMBD3DPdfData::CreateAttachSTEP242 Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMBD3DPdfData~CreateAttachSTEP242.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0