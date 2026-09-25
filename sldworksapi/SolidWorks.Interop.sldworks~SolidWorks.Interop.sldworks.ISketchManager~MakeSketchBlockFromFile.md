<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchBlockFromFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MakeSketchBlockFromFile Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : MakeSketchBlockFromFile Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*InsertionPoint*
:   [Insertion point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html), which is a 2D point with z = 0.0, for the block definition

*FileName*
:   Name of the external file to use to create the block definition

*LinkedToFile*
:   True to link the block definition to the file, false to not

*Scale*
:   Scale for the block definition

*Angle*
:   Rotation angle for the block definition

Creates a block definition using the specified file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MakeSketchBlockFromFile( _    ByVal InsertionPoint As MathPoint, _    ByVal FileName As System.String, _    ByVal LinkedToFile As System.Boolean, _    ByVal Scale As System.Double, _    ByVal Angle As System.Double _ ) As SketchBlockDefinition ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim InsertionPoint As MathPoint Dim FileName As System.String Dim LinkedToFile As System.Boolean Dim Scale As System.Double Dim Angle As System.Double Dim value As SketchBlockDefinition   value = instance.MakeSketchBlockFromFile(InsertionPoint, FileName, LinkedToFile, Scale, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` SketchBlockDefinition MakeSketchBlockFromFile(     MathPoint InsertionPoint,    System.string FileName,    System.bool LinkedToFile,    System.double Scale,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchBlockDefinition^ MakeSketchBlockFromFile(  &   MathPoint^ InsertionPoint, &   System.String^ FileName, &   System.bool LinkedToFile, &   System.double Scale, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*InsertionPoint*
:   [Insertion point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html), which is a 2D point with z = 0.0, for the block definition

*FileName*
:   Name of the external file to use to create the block definition

*LinkedToFile*
:   True to link the block definition to the file, false to not

*Scale*
:   Scale for the block definition

*Angle*
:   Rotation angle for the block definition

#### Return Value

[Block definition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBlockDefinition.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::MakeSketchBlockFromFile.

# ![](dotnetimages/collapse.gif)Remarks

If the entities of a block are associated with one or more layers and those layers do not already exist in the drawing, then the layers are inserted in the drawing and the associations between the entities of the block and the layers are maintained.

The block instance is inserted on the current drawing layer.

See Block Definitions and Block Instances for details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::MakeSketchBlockFromSelected Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchBlockFromSelected.html)

[ISketchManager::MakeSketchBlockFromSketch Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~MakeSketchBlockFromSketch.html)

[ISketchBlockDefinition::FileName Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockDefinition~FileName.html)

[ISketchBlockDefinition::LinkToFile Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockDefinition~LinkToFile.html)

[ISketchBlockDefinition::Save Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockDefinition~Save.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0