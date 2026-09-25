<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaceHatch~UseMaterialHatch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UseMaterialHatch Property (IFaceHatch) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFaceHatch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaceHatch.html) : UseMaterialHatch Property (IFaceHatch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether this face hatch uses material crosshatch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property UseMaterialHatch As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFaceHatch Dim value As System.Boolean   instance.UseMaterialHatch = value   value = instance.UseMaterialHatch ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UseMaterialHatch {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UseMaterialHatch {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to use material crosshatch, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FaceHatch::UseMaterialHatch.

# ![](dotnetimages/collapse.gif)Example

[Get Face Hatch Data (C#)](Get_Face_Hatch_Data_Example_CSharp.htm)

[Get Face Hatch Data (VB.NET)](Get_Face_Hatch_Data_Example_VBNET.htm)

[Get Face Hatch Data (VBA)](Get_Face_Hatch_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Material crosshatches are valid for [section views](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrSection.html) and aligned section views only.

# ![](dotnetimages/collapse.gif)See Also

####

[IFaceHatch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaceHatch.html)

[IFaceHatch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFaceHatch_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP4, Revision Number 17.4