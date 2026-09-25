<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertFormToolFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertFormToolFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertFormToolFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Path*
:   Pathname of the forming tool part file in the Design Library

*Flip*
:   Whether to reverse the direction of the cut of the forming tool when inserted

*RotAngle*
:   Angle of the forming tool

*Config*
:   Name of the configuration of the forming tool to insert

*OverrideDoc*
:   True to override the document settings in **Tools > Options > Document Properties > Sheet Metal,** false to not

*ShowPunch*
:   True to display the cut of the forming tool when the part is flattened, false to not; valid only if OverrideDoc = true

*ShowProfile*
:   True to display the placement sketch of the forming tool when the part is flattened, false to not; valid only if OverrideDoc = true

*ShowCenter*
:   True to display the center mark where the forming tool is located in the flat pattern, false to not; valid only if OverrideDoc = true

*LinkToPart*
:   True to link the forming tool feature to its part in the Design Library, false to not

Inserts a forming tool from the Design Library into a sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertFormToolFeature( _    ByVal Path As System.String, _    ByVal Flip As System.Boolean, _    ByVal RotAngle As System.Double, _    ByVal Config As System.String, _    ByVal OverrideDoc As System.Boolean, _    ByVal ShowPunch As System.Boolean, _    ByVal ShowProfile As System.Boolean, _    ByVal ShowCenter As System.Boolean, _    ByVal LinkToPart As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Path As System.String Dim Flip As System.Boolean Dim RotAngle As System.Double Dim Config As System.String Dim OverrideDoc As System.Boolean Dim ShowPunch As System.Boolean Dim ShowProfile As System.Boolean Dim ShowCenter As System.Boolean Dim LinkToPart As System.Boolean Dim value As Feature   value = instance.InsertFormToolFeature(Path, Flip, RotAngle, Config, OverrideDoc, ShowPunch, ShowProfile, ShowCenter, LinkToPart) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertFormToolFeature(     System.string Path,    System.bool Flip,    System.double RotAngle,    System.string Config,    System.bool OverrideDoc,    System.bool ShowPunch,    System.bool ShowProfile,    System.bool ShowCenter,    System.bool LinkToPart ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertFormToolFeature(  &   System.String^ Path, &   System.bool Flip, &   System.double RotAngle, &   System.String^ Config, &   System.bool OverrideDoc, &   System.bool ShowPunch, &   System.bool ShowProfile, &   System.bool ShowCenter, &   System.bool LinkToPart ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Path*
:   Pathname of the forming tool part file in the Design Library

*Flip*
:   Whether to reverse the direction of the cut of the forming tool when inserted

*RotAngle*
:   Angle of the forming tool

*Config*
:   Name of the configuration of the forming tool to insert

*OverrideDoc*
:   True to override the document settings in **Tools > Options > Document Properties > Sheet Metal,** false to not

*ShowPunch*
:   True to display the cut of the forming tool when the part is flattened, false to not; valid only if OverrideDoc = true

*ShowProfile*
:   True to display the placement sketch of the forming tool when the part is flattened, false to not; valid only if OverrideDoc = true

*ShowCenter*
:   True to display the center mark where the forming tool is located in the flat pattern, false to not; valid only if OverrideDoc = true

*LinkToPart*
:   True to link the forming tool feature to its part in the Design Library, false to not

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertFormToolFeature.

# ![](dotnetimages/collapse.gif)Example

[Insert Forming Tool Feature (VBA)](Insert_Form_Tool_Feature_Example_VB.htm)

[Insert Forming Tool Feature (VB.NET)](Insert_Form_Tool_Feature_Example_VBNET.htm)

[Insert Forming Tool Feature (C#)](Insert_Form_Tool_Feature_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, select either a face or a 2D sketch containing points. If you select:

* face, a single instance of the Design Library forming tool is placed on it.* sketch containing points, an instance of the Design Library forming tool is placed at each point in the sketch.

To create your own forming tool, call [IFeatureManager::CreateFormTool](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~CreateFormTool.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IView::InsertPunchTable Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertPunchTable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0