<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~AddCornerReliefType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddCornerReliefType Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : AddCornerReliefType Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CornerIndex*
:   Index of corner to which to apply the corner relief; -1 to apply it to the corner last added with [IFeatureManager::AddCornerReliefCorner](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~AddCornerReliefCorner.html)

*ReliefType*
:   Type of corner relief as defined by swCornerReliefType\_e

*Length1*
:   Not used

*Length2*
:   | If ReliefType is swCornerReliefType\_e... | Then Length2 is the slot... |
    | --- | --- |
    | swCornerSquareRelief | Length of the corner relief |
    | swCornerObroundRelief | Length of the corner relief |
    | swCornerCircularRelief | Radius of the corner relief |

*Length3*
:   | If ReliefType is swCornerReliefType\_e... | Then Length3 is... |
    | --- | --- |
    | swCornerObroundRelief | Slot width of the corner relief |
    | swCornerSquareRelief and FilletedCorners = true | Radius of filleted corner |

*CenterOnBendLines*
:   True to center the corner relief relative to the bend lines, false to not; valid only if ReliefType is one of the following:

    * swCornerReliefType\_e.swCornerSquareRelief* swCornerReliefType\_e.swCornerCircularRelief* swCornerReliefType\_e.swCornerObroundRelief

*RatioToThickness*
:   True to use a ratio value to cut the bend area so that the body can be folded, false to not; the ratios for valid relief types are calculated as follows where t = thickness of sheet metal:

    | If ReliefType is swCornerReliefType\_e... | Then ratios are... |
    | --- | --- |
    | swCornerSquareRelief | Length2/t |
    | swCornerCircularRelief | Length2/t |
    | swCornerObroundRelief | Length2/t and Length3/t |

*TangentToBend*
:   True to make the corner relief tangent to the inside bend edges, false to not

*AddFilletedCorners*
:   True to fillet the corner relief corners, false to not; valid only if ReliefType = swCornerReliefType\_e.swCornerSquareRelief

*NarrowCorner*
:   True to use the algorithm for large bend radii to narrow the corner relief in the bend area, false to not; valid only if ReliefType is one of the following:

    * swCornerReliefType\_e.swCornerSquareRelief* swCornerReliefType\_e.swCornerCircularRelief* swCornerReliefType\_e.swCornerObroundRelief

Specifies the type of corner relief to apply to the specified corner of the selected sheet metal body.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCornerReliefType( _    ByVal CornerIndex As System.Integer, _    ByVal ReliefType As System.Integer, _    ByVal Length1 As System.Double, _    ByVal Length2 As System.Double, _    ByVal Length3 As System.Double, _    ByVal CenterOnBendLines As System.Boolean, _    ByVal RatioToThickness As System.Boolean, _    ByVal TangentToBend As System.Boolean, _    ByVal AddFilletedCorners As System.Boolean, _    ByVal NarrowCorner As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim CornerIndex As System.Integer Dim ReliefType As System.Integer Dim Length1 As System.Double Dim Length2 As System.Double Dim Length3 As System.Double Dim CenterOnBendLines As System.Boolean Dim RatioToThickness As System.Boolean Dim TangentToBend As System.Boolean Dim AddFilletedCorners As System.Boolean Dim NarrowCorner As System.Boolean Dim value As System.Boolean   value = instance.AddCornerReliefType(CornerIndex, ReliefType, Length1, Length2, Length3, CenterOnBendLines, RatioToThickness, TangentToBend, AddFilletedCorners, NarrowCorner) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddCornerReliefType(     System.int CornerIndex,    System.int ReliefType,    System.double Length1,    System.double Length2,    System.double Length3,    System.bool CenterOnBendLines,    System.bool RatioToThickness,    System.bool TangentToBend,    System.bool AddFilletedCorners,    System.bool NarrowCorner ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddCornerReliefType(  &   System.int CornerIndex, &   System.int ReliefType, &   System.double Length1, &   System.double Length2, &   System.double Length3, &   System.bool CenterOnBendLines, &   System.bool RatioToThickness, &   System.bool TangentToBend, &   System.bool AddFilletedCorners, &   System.bool NarrowCorner ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CornerIndex*
:   Index of corner to which to apply the corner relief; -1 to apply it to the corner last added with [IFeatureManager::AddCornerReliefCorner](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~AddCornerReliefCorner.html)

*ReliefType*
:   Type of corner relief as defined by swCornerReliefType\_e

*Length1*
:   Not used

*Length2*
:   | If ReliefType is swCornerReliefType\_e... | Then Length2 is the slot... |
    | --- | --- |
    | swCornerSquareRelief | Length of the corner relief |
    | swCornerObroundRelief | Length of the corner relief |
    | swCornerCircularRelief | Radius of the corner relief |

*Length3*
:   | If ReliefType is swCornerReliefType\_e... | Then Length3 is... |
    | --- | --- |
    | swCornerObroundRelief | Slot width of the corner relief |
    | swCornerSquareRelief and FilletedCorners = true | Radius of filleted corner |

*CenterOnBendLines*
:   True to center the corner relief relative to the bend lines, false to not; valid only if ReliefType is one of the following:

    * swCornerReliefType\_e.swCornerSquareRelief* swCornerReliefType\_e.swCornerCircularRelief* swCornerReliefType\_e.swCornerObroundRelief

*RatioToThickness*
:   True to use a ratio value to cut the bend area so that the body can be folded, false to not; the ratios for valid relief types are calculated as follows where t = thickness of sheet metal:

    | If ReliefType is swCornerReliefType\_e... | Then ratios are... |
    | --- | --- |
    | swCornerSquareRelief | Length2/t |
    | swCornerCircularRelief | Length2/t |
    | swCornerObroundRelief | Length2/t and Length3/t |

*TangentToBend*
:   True to make the corner relief tangent to the inside bend edges, false to not

*AddFilletedCorners*
:   True to fillet the corner relief corners, false to not; valid only if ReliefType = swCornerReliefType\_e.swCornerSquareRelief

*NarrowCorner*
:   True to use the algorithm for large bend radii to narrow the corner relief in the bend area, false to not; valid only if ReliefType is one of the following:

    * swCornerReliefType\_e.swCornerSquareRelief* swCornerReliefType\_e.swCornerCircularRelief* swCornerReliefType\_e.swCornerObroundRelief

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::AddCornerReliefType.

# ![](dotnetimages/collapse.gif)Example

[Create Corner Relief Feature (C#)](Create_Corner_Relief_Feature_Example_CSharp.htm)

[Create Corner Relief Feature (VBA)](Create_Corner_Relief_Feature_Example_VB.htm)

[Create Corner Relief Feature (VB.NET)](Create_Corner_Relief_Feature_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

To create a corner relief feature:

1. Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 0 and Append = true to select the sheet metal body in which to create a corner relief feature.- Call IModelDocExtension::SelectByID2 with Mark = 4 and Append = true to select two faces that form a bend corner.- Call [IFeatureManager::AddCornerReliefCorner](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~AddCornerReliefCorner.html) to add the corner to the corner relief feature.- Call this method to specify the corner relief for the corner.- Repeat steps 2 - 4 to add another corner to the corner relief feature.- Call [IFeatureManager::FinishCornerRelief](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FinishCornerRelief.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFlatPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFlatPatternFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0