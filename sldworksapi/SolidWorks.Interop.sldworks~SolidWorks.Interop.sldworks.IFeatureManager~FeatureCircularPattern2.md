<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCircularPattern2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureCircularPattern2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureCircularPattern2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Num*
:   Number of instances of the circular pattern to insert, including the original

*Spacing*
:   Spacing between each instance of the circular pattern in radians

*FlipDir*
:   True to flip the direction of the circular pattern, false to not

*DName*
:   Name of the angular dimension defining the direction of the pattern

*GeometryPattern*
:   True to use geometry pattern, false to not

Obsolete. Superseded by [IFeatureManager::FeatureCircularPattern3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~FeatureCircularPattern3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureCircularPattern2( _    ByVal Num As System.Integer, _    ByVal Spacing As System.Double, _    ByVal FlipDir As System.Boolean, _    ByVal DName As System.String, _    ByVal GeometryPattern As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Num As System.Integer Dim Spacing As System.Double Dim FlipDir As System.Boolean Dim DName As System.String Dim GeometryPattern As System.Boolean Dim value As Feature   value = instance.FeatureCircularPattern2(Num, Spacing, FlipDir, DName, GeometryPattern) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureCircularPattern2(     System.int Num,    System.double Spacing,    System.bool FlipDir,    System.string DName,    System.bool GeometryPattern ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureCircularPattern2(  &   System.int Num, &   System.double Spacing, &   System.bool FlipDir, &   System.String^ DName, &   System.bool GeometryPattern ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Num*
:   Number of instances of the circular pattern to insert, including the original

*Spacing*
:   Spacing between each instance of the circular pattern in radians

*FlipDir*
:   True to flip the direction of the circular pattern, false to not

*DName*
:   Name of the angular dimension defining the direction of the pattern

*GeometryPattern*
:   True to use geometry pattern, false to not

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureCircularPattern2.

# ![](dotnetimages/collapse.gif)Remarks

This method requires ordered selection of the features and components.

* Features and axis: Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) with a Mark of 4 for the features to pattern and a Mark of 1 for the axis. You can also use [IFeature::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~Select2.html) to select the features and the axis.

  * Components and axis: Use IModelDocExtension::SelectByID2 with a Mark of 1 for the components to pattern and a Mark of 2 for the axis.

You must select the features or components before selecting the axis.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ICircularPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICircularPatternFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0