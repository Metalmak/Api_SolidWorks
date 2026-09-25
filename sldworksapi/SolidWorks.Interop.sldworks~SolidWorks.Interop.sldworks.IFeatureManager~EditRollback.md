<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~EditRollback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditRollback Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : EditRollback Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Location*
:   Location to which to move the rollback bar as defined in swMoveRollbackBarTo\_e

*Feature*
:   Name of the feature

Rolls back or forward the rollback bar to a specific location in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditRollback( _    ByVal Location As System.Integer, _    ByVal Feature As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Location As System.Integer Dim Feature As System.String Dim value As System.Boolean   value = instance.EditRollback(Location, Feature) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EditRollback(     System.int Location,    System.string Feature ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool EditRollback(  &   System.int Location, &   System.String^ Feature ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Location*
:   Location to which to move the rollback bar as defined in swMoveRollbackBarTo\_e

*Feature*
:   Name of the feature

#### Return Value

True if moving the rollback bar back or forward was successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::EditRollback.

# ![](dotnetimages/collapse.gif)Example

[Roll Back Model (C#)](Roll_Back_Model_Example_CSharp.htm)

[Roll Back Model (VB.NET)](Roll_Back_Model_Example_VBNET.htm)

[Roll Back Model (VBA)](Roll_Back_Model_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

When the model is in a rollback state, it reverts to an earlier state, suppressing recently added features. You can add new features or edit existing features while the model is in the rolled-back state.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeature::IsRolledBack Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsRolledBack.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0