<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy~SaveToAVI.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| SaveToAVI Method (IMotionStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) > [IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html) : SaveToAVI Method (IMotionStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Path and filename where to save a .avi, .bmp, or .tga file

*Parameter*
:   [Parameters](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IAVIParameter.html) for the .avi file

Saves the animation to a .avi, .bmp, or .tga file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SaveToAVI( _    ByVal FileName As System.String, _    ByVal Parameter As AVIParameter _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMotionStudy Dim FileName As System.String Dim Parameter As AVIParameter Dim value As System.Boolean   value = instance.SaveToAVI(FileName, Parameter) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SaveToAVI(     System.string FileName,    AVIParameter Parameter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SaveToAVI(  &   System.String^ FileName, &   AVIParameter^ Parameter ) ``` | |

#### Parameters

*FileName*
:   Path and filename where to save a .avi, .bmp, or .tga file

*Parameter*
:   [Parameters](SOLIDWORKS.Interop.swmotionstudy~SOLIDWORKS.Interop.swmotionstudy.IAVIParameter.html) for the .avi file

#### Return Value

True if the animation is saved to the specified file, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MotionStudy::SaveToAVI.

# ![](dotnetimages/collapse.gif)Example

[Duplicate, Delete, and Create Motion Study (C#)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_CSharp.htm)

[Duplicate, Delete, and Create Motion Study (VB.NET)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_VBNET.htm)

[Duplicate, Delete, and Create Motion Study (VBA)](Duplicate%2C_Delete%2C_and_Create_Motion_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IMotionStudy Interface](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy.html)

[IMotionStudy Members](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IMotionStudy_members.html)

[IAVIParameter::MotionBlur Property ()](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.IAVIParameter~MotionBlur.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0