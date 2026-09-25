<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertMoveFace2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertMoveFace2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : IInsertMoveFace2 Method (IFeatureManager) |

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

*TranslationParams*
:   * in-process, unmanaged C++: Pointer to an array three doubles for delta x, delta y, and delta z direction translation

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*RotationParams*
:   * in-process, unmanaged C++: Pointer to an array six doubles:
      + first three doubles are the x, y, and z rotation origin+ last three doubles are the x, y, and z rotation angle

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

Obsolete. Superseded by [IFeatureManager::InsertMoveFace3.](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoveFace3.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertMoveFace2( _    ByVal MoveType As System.Integer, _    ByVal ReverseDir As System.Boolean, _    ByVal Angle As System.Double, _    ByVal Distance As System.Double, _    ByRef TranslationParams As System.Double, _    ByRef RotationParams As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim MoveType As System.Integer Dim ReverseDir As System.Boolean Dim Angle As System.Double Dim Distance As System.Double Dim TranslationParams As System.Double Dim RotationParams As System.Double Dim value As Feature   value = instance.IInsertMoveFace2(MoveType, ReverseDir, Angle, Distance, TranslationParams, RotationParams) ``` | |

| C# |  |
| --- | --- |
| ``` Feature IInsertMoveFace2(     System.int MoveType,    System.bool ReverseDir,    System.double Angle,    System.double Distance,    ref System.double TranslationParams,    ref System.double RotationParams ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ IInsertMoveFace2(  &   System.int MoveType, &   System.bool ReverseDir, &   System.double Angle, &   System.double Distance, &   System.double% TranslationParams, &   System.double% RotationParams ) ``` | |

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

*TranslationParams*
:   * in-process, unmanaged C++: Pointer to an array three doubles for delta x, delta y, and delta z direction translation

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

*RotationParams*
:   * in-process, unmanaged C++: Pointer to an array six doubles:
      + first three doubles are the x, y, and z rotation origin+ last three doubles are the x, y, and z rotation angle

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Remarks

Use the following marks with [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html):

* 1 = face

  * 2 = direction reference (plane, planar face, linear edge, or reference axis) for translate

    * 4 = axis reference (linear edge or reference axis) for rotate

If you specify a value for TranslationParms or RotationParams, then do not specify a value for Distance or Angle, respectively. The translation or rotation parameters are calculated internally when Distance or Angle is specified.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IMoveFaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData.html)

[IFeatureManager::InsertMoveFace2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMoveFace2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0