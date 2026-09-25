<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertGeneralToleranceTableAnnotation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertGeneralToleranceTableAnnotation Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : InsertGeneralToleranceTableAnnotation Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplateName*
:   Path and file name of the table template to use (see **Remarks**)

*X*
:   X coordinate of this table annotation

*Y*
:   Y coordinate of this table annotation

Inserts a general tolerance table annotation in this model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertGeneralToleranceTableAnnotation( _    ByVal TemplateName As System.String, _    ByVal X As System.Integer, _    ByVal Y As System.Integer _ ) As GeneralToleranceTableAnnotation ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim TemplateName As System.String Dim X As System.Integer Dim Y As System.Integer Dim value As GeneralToleranceTableAnnotation   value = instance.InsertGeneralToleranceTableAnnotation(TemplateName, X, Y) ``` | |

| C# |  |
| --- | --- |
| ``` GeneralToleranceTableAnnotation InsertGeneralToleranceTableAnnotation(     System.string TemplateName,    System.int X,    System.int Y ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` GeneralToleranceTableAnnotation^ InsertGeneralToleranceTableAnnotation(  &   System.String^ TemplateName, &   System.int X, &   System.int Y ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TemplateName*
:   Path and file name of the table template to use (see **Remarks**)

*X*
:   X coordinate of this table annotation

*Y*
:   Y coordinate of this table annotation

#### Return Value

[IGeneralToleranceTableAnnotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralToleranceTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::InsertGeneralToleranceTableAnnotation.

# ![](dotnetimages/collapse.gif)Example

[Insert General Tolerance Table (VBA)](Insert_General_Tolerance_Table_Example_VB.htm)

[Insert General Tolerance Table (VB.NET)](Insert_General_Tolerance_Table_Example_VBNET.htm)

[Insert General Tolerance Table (C#)](Insert_General_Tolerance_Table_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Specify TemplateName with *install\_dir***\lang\***lang***\bom-standard.sldbomtbt**.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IGeneralToleranceTableFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGeneralToleranceTableFeature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0