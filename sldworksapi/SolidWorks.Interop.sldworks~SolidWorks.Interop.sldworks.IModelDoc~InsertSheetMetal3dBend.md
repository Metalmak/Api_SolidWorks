<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~InsertSheetMetal3dBend.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSheetMetal3dBend Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : InsertSheetMetal3dBend Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Angle*

*Radius*

*FlipDir*

*BendPos*

Obsolete. Superseded by [IModelDoc2::InsertSheetMetal3dBend](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~InsertSheetMetal3dBend.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub InsertSheetMetal3dBend( _    ByVal Angle As System.Double, _    ByVal Radius As System.Double, _    ByVal FlipDir As System.Boolean, _    ByVal BendPos As System.Short _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Angle As System.Double Dim Radius As System.Double Dim FlipDir As System.Boolean Dim BendPos As System.Short   instance.InsertSheetMetal3dBend(Angle, Radius, FlipDir, BendPos) ``` | |

| C# |  |
| --- | --- |
| ``` void InsertSheetMetal3dBend(     System.double Angle,    System.double Radius,    System.bool FlipDir,    System.short BendPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void InsertSheetMetal3dBend(  &   System.double Angle, &   System.double Radius, &   System.bool FlipDir, &   System.short BendPos ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Angle*

*Radius*

*FlipDir*

*BendPos*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::InsertSheetMetal3dBend.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)