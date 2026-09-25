<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~MoveFreezeBarTo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoveFreezeBarTo2 Method (IFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : MoveFreezeBarTo2 Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Location*
:   * swMoveFreezeBarTo\_e.swMoveFreezeBarToBeforeFeature

      -or-

    * swMoveFreezeBarTo\_e.swMoveFreezeBarToAfterFeature

*UpdateAllConfigs*
:   True to update all configurations, false to not

*UnlockConfigs*
:   True to unlock configurations, false to not

Moves the freeze bar to the specified location in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MoveFreezeBarTo2( _    ByVal Location As System.Integer, _    ByVal UpdateAllConfigs As System.Boolean, _    ByVal UnlockConfigs As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim Location As System.Integer Dim UpdateAllConfigs As System.Boolean Dim UnlockConfigs As System.Boolean Dim value As System.Integer   value = instance.MoveFreezeBarTo2(Location, UpdateAllConfigs, UnlockConfigs) ``` | |

| C# |  |
| --- | --- |
| ``` System.int MoveFreezeBarTo2(     System.int Location,    System.bool UpdateAllConfigs,    System.bool UnlockConfigs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int MoveFreezeBarTo2(  &   System.int Location, &   System.bool UpdateAllConfigs, &   System.bool UnlockConfigs ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Location*
:   * swMoveFreezeBarTo\_e.swMoveFreezeBarToBeforeFeature

      -or-

    * swMoveFreezeBarTo\_e.swMoveFreezeBarToAfterFeature

*UpdateAllConfigs*
:   True to update all configurations, false to not

*UnlockConfigs*
:   True to unlock configurations, false to not

#### Return Value

0 indicates that the freeze bar did not move to the specified location in the FeatureManager design tree; a non-0 value indicates that the freeze bar did move to the specified location in the FeatureManager design tree

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::MoveFreezeBarTo2.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IFeature::IsFrozen Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsFrozen.html)

[IFeature::HasFrozenUpdatePending Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~HasFrozenUpdatePending.html)

[IFeature::IsHiddenLock Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IsHiddenLock.html)

[IFeatureManager::EditFreeze2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~EditFreeze2.html)

[IFeatureManager::GetFreezeLocation Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~GetFreezeLocation.html)

[IModelDocExtension::UpdateFrozenFeatures Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateFrozenFeatures.html)

[IModelDocExtension::NeedsRebuild2 Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~NeedsRebuild2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0