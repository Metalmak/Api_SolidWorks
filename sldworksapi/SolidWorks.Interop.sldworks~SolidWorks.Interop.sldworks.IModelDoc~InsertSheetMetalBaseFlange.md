<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertSheetMetalBaseFlange.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetalBaseFlange Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertSheetMetalBaseFlange Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Thickness*

*ThickenDir*

*Radius*

*ExtrudeDist1*

*ExtrudeDist2*

*FlipExtruDir*

*EndCondition1*

*EndCondition2*

*DirToUse*

Obsolete. Superseded by [IModelDoc2::InsertSheetMetalBaseFlange](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertSheetMetalBaseFlange.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertSheetMetalBaseFlange( _    ByVal Thickness As System.Double, _    ByVal ThickenDir As System.Boolean, _    ByVal Radius As System.Double, _    ByVal ExtrudeDist1 As System.Double, _    ByVal ExtrudeDist2 As System.Double, _    ByVal FlipExtruDir As System.Boolean, _    ByVal EndCondition1 As System.Integer, _    ByVal EndCondition2 As System.Integer, _    ByVal DirToUse As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Thickness As System.Double Dim ThickenDir As System.Boolean Dim Radius As System.Double Dim ExtrudeDist1 As System.Double Dim ExtrudeDist2 As System.Double Dim FlipExtruDir As System.Boolean Dim EndCondition1 As System.Integer Dim EndCondition2 As System.Integer Dim DirToUse As System.Integer   instance.InsertSheetMetalBaseFlange(Thickness, ThickenDir, Radius, ExtrudeDist1, ExtrudeDist2, FlipExtruDir, EndCondition1, EndCondition2, DirToUse) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertSheetMetalBaseFlange(     System.double Thickness,    System.bool ThickenDir,    System.double Radius,    System.double ExtrudeDist1,    System.double ExtrudeDist2,    System.bool FlipExtruDir,    System.int EndCondition1,    System.int EndCondition2,    System.int DirToUse ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertSheetMetalBaseFlange(  &   System.double Thickness, &   System.bool ThickenDir, &   System.double Radius, &   System.double ExtrudeDist1, &   System.double ExtrudeDist2, &   System.bool FlipExtruDir, &   System.int EndCondition1, &   System.int EndCondition2, &   System.int DirToUse ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Thickness*

*ThickenDir*

*Radius*

*ExtrudeDist1*

*ExtrudeDist2*

*FlipExtruDir*

*EndCondition1*

*EndCondition2*

*DirToUse*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertSheetMetalBaseFlange.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)