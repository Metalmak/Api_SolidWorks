<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~LargeDesignReviewMark.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LargeDesignReviewMark Property (IConfiguration) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html) : LargeDesignReviewMark Property (IConfiguration) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to generate a display list for this configuration when the document is saved.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property LargeDesignReviewMark As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IConfiguration Dim value As System.Boolean   instance.LargeDesignReviewMark = value   value = instance.LargeDesignReviewMark ``` | |

| C# |  |
| --- | --- |
| ``` System.bool LargeDesignReviewMark {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool LargeDesignReviewMark {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to add display data, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Configuration::LargeDesignReviewMark.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Large Design Review Marks for Configurations (C#)](Get_and_Set_Large_Design_Review_Marks_for_Configurations_Example_CSharp.htm)

[Get and Set Large Design Review Marks for Configurations (VB.NET)](Get_and_Set_Large_Design_Review_Marks_for_Configurations_Example_VBNET.htm)

[Get and Set Large Design Review Marks for Configurations (VBA)](Get_and_Set_Large_Design_Review_Marks_for_Configurations_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if this configuration is one of multiple configurations defined for the assembly or part.

Before SOLIDWORKS 2019, this property specified whether to generate a display list for the configuration of an assembly when it is saved. As of SOLIDWORKS 2019, this property specifies whether to generate a display list for this configuration of:

* an assembly on save. If this property is set to true, the assembly configuration's display list is saved, making the configuration visible in Large Design Review mode. In the user interface, this corresponds to selecting the assembly's **ConfigurationManager >** *configuration\_name* **RMB menu > Add Display Data Mark**.

   - or -

* a part on save. If this property is set to true, the part configuration's display list is saved, making the configuration visible in other applications, such as eDrawings. In the user interface, this corresponds to selecting the part's **ConfigurationManager >** *configuration\_name* **RMB menu > Add Display Data Mark**.

# ![](dotnetimages/collapse.gif)See Also

####

[IConfiguration Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration.html)

[IConfiguration Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration_members.html)

[IDocumentSpecification::ViewOnly Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~ViewOnly.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0