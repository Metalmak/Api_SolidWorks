<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoveFace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMoveFace Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMoveFace Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MoveType*
:   Type of move:

    * 0 = Offset

      * 1 = Translate

        * 2 = Rotate

*ReverseDir*
:   True to reverse the direction, false to not

*Angle*
:   If MoveType is Rotate, then specify the angle at which to draft the faces

*Distance*
:   Distance to offset or translate the faces

Obsolete. Superseded by [IFeatureManager::InsertMoveFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertMoveFace2.html) and [IFeatureManager::IInsertMoveFace2.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~IInsertMoveFace2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMoveFace( _    ByVal MoveType As System.Integer, _    ByVal ReverseDir As System.Boolean, _    ByVal Angle As System.Double, _    ByVal Distance As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim MoveType As System.Integer Dim ReverseDir As System.Boolean Dim Angle As System.Double Dim Distance As System.Double Dim value As Feature   value = instance.InsertMoveFace(MoveType, ReverseDir, Angle, Distance) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMoveFace(     System.int MoveType,    System.bool ReverseDir,    System.double Angle,    System.double Distance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMoveFace(  &   System.int MoveType, &   System.bool ReverseDir, &   System.double Angle, &   System.double Distance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MoveType*
:   Type of move:

    * 0 = Offset

      * 1 = Translate

        * 2 = Rotate

*ReverseDir*
:   True to reverse the direction, false to not

*Angle*
:   If MoveType is Rotate, then specify the angle at which to draft the faces

*Distance*
:   Distance to offset or translate the faces

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMoveFace.

# ![](dotnetimages/collapse.gif)Example

[Move Selected Face (VBA)](Move_Selected_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use the following marks with [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html):

* 1 = face

  * 2 = direction reference (plane, planar face, linear edge, or reference axis) for translate

    * 4 = axis reference (linear edge or reference axis) for rotate

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IMoveFaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0