<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoveFace3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMoveFace3 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMoveFace3 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MoveType*
:   Type of move as defined in swMoveFaceType\_e

*ReverseDir*
:   True to reverse the direction, false to not

*Angle*
:   Angle at which to draft the faces; valid only if MoveType is swMoveFaceType\_e.swMoveFaceTypeRotate (see **Remarks**)

*Distance*
:   Distance to translate or offset the faces; valid only if MoveType is one of the following:

    * swMoveFaceType\_e.swMoveFaceTypeOffset* swMoveFaceType\_e.swMoveFaceTypeTranslate and EndConditionType is swEndConditions\_e.swEndCondBlind (see **Remarks**)

*TranslationParams*
:   Array of three doubles for the delta x, delta y, and delta z direction translation (see **Remarks**)

*RotationParams*
:   Array of six doubles:

    * First three doubles are the x, y, and z rotation origin* Last three doubles are the x, y, and z rotation angle

    (see **Remarks**)

*EndConditionType*
:   End condition as defined in swEndConditions\_e; valid only if MoveType is swMoveFaceType\_e.swMoveFaceTypeTranslate

    Only the following end condition types are valid:

    * swEndConditions\_e.swEndCondBlind* swEndConditions\_e.swEndCondUpToVertex* swEndConditions\_e.swEndCondUpToSurface* swEndConditions\_e.swEndCondOffsetFromSurface* swEndConditions\_e.swEndCondUpToBody

*OffsetDistance*
:   Offset from surface; valid only if MoveType is swMoveFaceType\_e.swMoveFaceTypeTranslate and EndConditionType is swEndConditions\_e.swEndCondOffsetFromSurface

Moves the selected faces on a solid or surface model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMoveFace3( _    ByVal MoveType As System.Integer, _    ByVal ReverseDir As System.Boolean, _    ByVal Angle As System.Double, _    ByVal Distance As System.Double, _    ByVal TranslationParams As System.Object, _    ByVal RotationParams As System.Object, _    ByVal EndConditionType As System.Integer, _    ByVal OffsetDistance As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim MoveType As System.Integer Dim ReverseDir As System.Boolean Dim Angle As System.Double Dim Distance As System.Double Dim TranslationParams As System.Object Dim RotationParams As System.Object Dim EndConditionType As System.Integer Dim OffsetDistance As System.Double Dim value As Feature   value = instance.InsertMoveFace3(MoveType, ReverseDir, Angle, Distance, TranslationParams, RotationParams, EndConditionType, OffsetDistance) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMoveFace3(     System.int MoveType,    System.bool ReverseDir,    System.double Angle,    System.double Distance,    System.object TranslationParams,    System.object RotationParams,    System.int EndConditionType,    System.double OffsetDistance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMoveFace3(  &   System.int MoveType, &   System.bool ReverseDir, &   System.double Angle, &   System.double Distance, &   System.Object^ TranslationParams, &   System.Object^ RotationParams, &   System.int EndConditionType, &   System.double OffsetDistance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MoveType*
:   Type of move as defined in swMoveFaceType\_e

*ReverseDir*
:   True to reverse the direction, false to not

*Angle*
:   Angle at which to draft the faces; valid only if MoveType is swMoveFaceType\_e.swMoveFaceTypeRotate (see **Remarks**)

*Distance*
:   Distance to translate or offset the faces; valid only if MoveType is one of the following:

    * swMoveFaceType\_e.swMoveFaceTypeOffset* swMoveFaceType\_e.swMoveFaceTypeTranslate and EndConditionType is swEndConditions\_e.swEndCondBlind (see **Remarks**)

*TranslationParams*
:   Array of three doubles for the delta x, delta y, and delta z direction translation (see **Remarks**)

*RotationParams*
:   Array of six doubles:

    * First three doubles are the x, y, and z rotation origin* Last three doubles are the x, y, and z rotation angle

    (see **Remarks**)

*EndConditionType*
:   End condition as defined in swEndConditions\_e; valid only if MoveType is swMoveFaceType\_e.swMoveFaceTypeTranslate

    Only the following end condition types are valid:

    * swEndConditions\_e.swEndCondBlind* swEndConditions\_e.swEndCondUpToVertex* swEndConditions\_e.swEndCondUpToSurface* swEndConditions\_e.swEndCondOffsetFromSurface* swEndConditions\_e.swEndCondUpToBody

*OffsetDistance*
:   Offset from surface; valid only if MoveType is swMoveFaceType\_e.swMoveFaceTypeTranslate and EndConditionType is swEndConditions\_e.swEndCondOffsetFromSurface

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMoveFace3.

# ![](dotnetimages/collapse.gif)Example

[Create and Modify Move Face Feature (VBA)](Create_and_Modify_Move_Face_Feature_Example_VB.htm)

[Create and Modify Move Face Feature (VB.NET)](Create_and_Modify_Move_Face_Feature_Example_VBNET.htm)

[Create and Modify Move Face Feature (C#)](Create_and_Modify_Move_Face_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you need to select specific entities.

| If MoveFaceType is swMoveFaceType\_e... | And EndConditionType is swEndConditions\_e... | Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select... | With mark... |
| --- | --- | --- | --- |
| Any option | Any option | Face to move | 1 |
| swMoveFaceTypeTranslate | Any option | Direction reference (plane, planar face, linear edge, or reference axis) | 2 |
| swMoveFaceTypeTranslate | * swEndCondUpToVertex* swEndCondUpToSurface* swEndCondOffsetFromSurface* swEndCondUpToBody | * Up-to vertex* Up-to surface* Offset-from surface* Up-to body | 8 |
| swMoveFaceTypeRotate | N/A | Axis reference (linear edge or reference axis) | 4 |

If you specify a value for TranslationParms or RotationParams, then do not specify a value for Distance or Angle, respectively. The translation or rotation parameters are calculated internally when Distance or Angle is specified.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IMoveFaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0