<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWeldmentTrimFeature2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertWeldmentTrimFeature2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertWeldmentTrimFeature2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EndCond*
:   End condition as defined by swSolidworksWeldmentEndCondOptions\_e

*Options*
:   Logical sum of values as defined in swWeldmentTrimExtendOptionType\_e (see **Remarks**)

*GapValue*
:   Length to trim (see **Remarks**)

*BodiesToTrim*
:   Array of bodies to trim

*BodiesOrFaces*
:   Array of bodies or faces that define the trimming boundaries

Inserts a weldment trim feature for the specified weldment bodies or faces.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertWeldmentTrimFeature2( _    ByVal EndCond As System.Integer, _    ByVal Options As System.Integer, _    ByVal GapValue As System.Double, _    ByVal BodiesToTrim As System.Object, _    ByVal BodiesOrFaces As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim EndCond As System.Integer Dim Options As System.Integer Dim GapValue As System.Double Dim BodiesToTrim As System.Object Dim BodiesOrFaces As System.Object Dim value As Feature   value = instance.InsertWeldmentTrimFeature2(EndCond, Options, GapValue, BodiesToTrim, BodiesOrFaces) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertWeldmentTrimFeature2(     System.int EndCond,    System.int Options,    System.double GapValue,    System.object BodiesToTrim,    System.object BodiesOrFaces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertWeldmentTrimFeature2(  &   System.int EndCond, &   System.int Options, &   System.double GapValue, &   System.Object^ BodiesToTrim, &   System.Object^ BodiesOrFaces ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EndCond*
:   End condition as defined by swSolidworksWeldmentEndCondOptions\_e

*Options*
:   Logical sum of values as defined in swWeldmentTrimExtendOptionType\_e (see **Remarks**)

*GapValue*
:   Length to trim (see **Remarks**)

*BodiesToTrim*
:   Array of bodies to trim

*BodiesOrFaces*
:   Array of bodies or faces that define the trimming boundaries

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertWeldmentTrimFeature2.

# ![](dotnetimages/collapse.gif)Example

[Insert Weldment Features (VBA)](Insert_Weldment_Features_Example_VB.htm)

[Insert Weldment Features (VB.NET)](Insert_Weldment_Features_Example_VBNET.htm)

[Insert Weldment Features (C#)](Insert_Weldment_Features_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) and specify the following marks to select the body, or bodies, to trim and the trimming boundaries:

* 1 = Body or bodies to trim* 2 = Trimming boundaries (body or face)

If you include swWeldmentTrimExtendOption\_WeldGap in the Options parameter, then the GapValue parameter is used. Specify 0 for GapValue to ensure that there is no weld gap.

If you exclude swWeldmentTrimExtendOption\_WeldGap from the Options parameter, then the weld gap defaults to the last value specified in the SOLIDWORKS user-interface.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertWeldmentTrimFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWeldmentTrimFeature.html)

[IWeldmentTrimExtendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentTrimExtendFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0