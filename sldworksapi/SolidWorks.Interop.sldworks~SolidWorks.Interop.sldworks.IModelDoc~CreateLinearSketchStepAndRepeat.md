<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~CreateLinearSketchStepAndRepeat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateLinearSketchStepAndRepeat Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : CreateLinearSketchStepAndRepeat Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumX*

*NumY*

*SpacingX*

*SpacingY*

*AngleX*

*AngleY*

*DeleteInstances*

Obsolete. Superseded by [IModelDoc2::CreateLinearSketchStepAndRepeat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~CreateLinearSketchStepAndRepeat.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateLinearSketchStepAndRepeat( _    ByVal NumX As System.Integer, _    ByVal NumY As System.Integer, _    ByVal SpacingX As System.Double, _    ByVal SpacingY As System.Double, _    ByVal AngleX As System.Double, _    ByVal AngleY As System.Double, _    ByVal DeleteInstances As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim NumX As System.Integer Dim NumY As System.Integer Dim SpacingX As System.Double Dim SpacingY As System.Double Dim AngleX As System.Double Dim AngleY As System.Double Dim DeleteInstances As System.String Dim value As System.Boolean   value = instance.CreateLinearSketchStepAndRepeat(NumX, NumY, SpacingX, SpacingY, AngleX, AngleY, DeleteInstances) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateLinearSketchStepAndRepeat(     System.int NumX,    System.int NumY,    System.double SpacingX,    System.double SpacingY,    System.double AngleX,    System.double AngleY,    System.string DeleteInstances ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateLinearSketchStepAndRepeat(  &   System.int NumX, &   System.int NumY, &   System.double SpacingX, &   System.double SpacingY, &   System.double AngleX, &   System.double AngleY, &   System.String^ DeleteInstances ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumX*

*NumY*

*SpacingX*

*SpacingY*

*AngleX*

*AngleY*

*DeleteInstances*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::CreateLinearSketchStepAndRepeat.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)