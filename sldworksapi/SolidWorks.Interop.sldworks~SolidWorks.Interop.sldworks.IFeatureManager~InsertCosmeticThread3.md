<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCosmeticThread3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCosmeticThread3 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertCosmeticThread3 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Standard*
:   Thread standard as defined by swCosmeticStandardType\_e

*StandardType*
:   Thread type for Standard

*Size*
:   Thread size for the specified Standard

*Diameter*
:   Thread diameter

*EndType*
:   End condition as defined by swCosmeticEndConditions\_e

*Depth*
:   Depth of the cosmetic thread; valid only for EndType = swCosmeticEndConditions\_e.swEndConditionBlind or swCosmeticEndConditions\_e.swEndConditionBlindUptoNext or swCosmeticEndConditions\_e.swEndConditionBlind2Dia

*Note*
:   Callout text to display in the drawing document

Inserts a cosmetic thread.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCosmeticThread3( _    ByVal Standard As System.Integer, _    ByVal StandardType As System.String, _    ByVal Size As System.String, _    ByVal Diameter As System.Double, _    ByVal EndType As System.Integer, _    ByVal Depth As System.Double, _    ByVal Note As System.String _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Standard As System.Integer Dim StandardType As System.String Dim Size As System.String Dim Diameter As System.Double Dim EndType As System.Integer Dim Depth As System.Double Dim Note As System.String Dim value As Feature   value = instance.InsertCosmeticThread3(Standard, StandardType, Size, Diameter, EndType, Depth, Note) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertCosmeticThread3(     System.int Standard,    System.string StandardType,    System.string Size,    System.double Diameter,    System.int EndType,    System.double Depth,    System.string Note ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertCosmeticThread3(  &   System.int Standard, &   System.String^ StandardType, &   System.String^ Size, &   System.double Diameter, &   System.int EndType, &   System.double Depth, &   System.String^ Note ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Standard*
:   Thread standard as defined by swCosmeticStandardType\_e

*StandardType*
:   Thread type for Standard

*Size*
:   Thread size for the specified Standard

*Diameter*
:   Thread diameter

*EndType*
:   End condition as defined by swCosmeticEndConditions\_e

*Depth*
:   Depth of the cosmetic thread; valid only for EndType = swCosmeticEndConditions\_e.swEndConditionBlind or swCosmeticEndConditions\_e.swEndConditionBlindUptoNext or swCosmeticEndConditions\_e.swEndConditionBlind2Dia

*Note*
:   Callout text to display in the drawing document

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertCosmeticThread3.

# ![](dotnetimages/collapse.gif)Example

[Traverse All Cosmetic Threads (VBA)](Traverse_All_Cosmetic_Threads_Example_VB.htm)

[Traverse All Cosmetic Threads (VB.NET)](Traverse_All_Cosmetic_Threads_Example_VBNET.htm)

[Traverse All Cosmetic Threads (C#)](Traverse_All_Cosmetic_Threads_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ICosmeticThreadFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICosmeticThreadFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0