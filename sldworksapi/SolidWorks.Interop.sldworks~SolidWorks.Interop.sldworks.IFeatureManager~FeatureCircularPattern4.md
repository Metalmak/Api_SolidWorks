<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCircularPattern4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureCircularPattern4 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureCircularPattern4 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Number*
:   Number of instances of the circular pattern to insert, including the original instance

*Spacing*
:   Spacing between each instance of the circular pattern; total angle in radians if EqualSpacing is true

*FlipDirection*
:   True to flip the direction of the circular pattern, false to not

*DName*
:   Name of the angular dimension defining the direction of the pattern

*GeometryPattern*
:   True to use geometry pattern, false to not

*EqualSpacing*
:   True to use equal spacing, false to not

*VaryInstance*
:   True to vary the dimensions or spacing of individual pattern instances, false to not; valid only if GeometryPattern = false (see **Remarks**)

Obsolete. Superseded by [IFeatureManager::FeatureCircularPattern5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCircularPattern5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureCircularPattern4( _    ByVal Number As System.Integer, _    ByVal Spacing As System.Double, _    ByVal FlipDirection As System.Boolean, _    ByVal DName As System.String, _    ByVal GeometryPattern As System.Boolean, _    ByVal EqualSpacing As System.Boolean, _    ByVal VaryInstance As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Number As System.Integer Dim Spacing As System.Double Dim FlipDirection As System.Boolean Dim DName As System.String Dim GeometryPattern As System.Boolean Dim EqualSpacing As System.Boolean Dim VaryInstance As System.Boolean Dim value As Feature   value = instance.FeatureCircularPattern4(Number, Spacing, FlipDirection, DName, GeometryPattern, EqualSpacing, VaryInstance) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureCircularPattern4(     System.int Number,    System.double Spacing,    System.bool FlipDirection,    System.string DName,    System.bool GeometryPattern,    System.bool EqualSpacing,    System.bool VaryInstance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureCircularPattern4(  &   System.int Number, &   System.double Spacing, &   System.bool FlipDirection, &   System.String^ DName, &   System.bool GeometryPattern, &   System.bool EqualSpacing, &   System.bool VaryInstance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Number*
:   Number of instances of the circular pattern to insert, including the original instance

*Spacing*
:   Spacing between each instance of the circular pattern; total angle in radians if EqualSpacing is true

*FlipDirection*
:   True to flip the direction of the circular pattern, false to not

*DName*
:   Name of the angular dimension defining the direction of the pattern

*GeometryPattern*
:   True to use geometry pattern, false to not

*EqualSpacing*
:   True to use equal spacing, false to not

*VaryInstance*
:   True to vary the dimensions or spacing of individual pattern instances, false to not; valid only if GeometryPattern = false (see **Remarks**)

#### Return Value

Circular pattern [feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureCircularPattern4.

# ![](dotnetimages/collapse.gif)Example

[Create Circular Pattern (VBA)](Create_Circular_Pattern_Example_VB.htm)

[Create Circular Pattern (VB.NET)](Create_Circular_Pattern_Example_VBNET.htm)

[Create Circular Pattern (C#)](Create_Circular_Pattern_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |  |
| --- | --- | --- |
| If... | To select a feature, use... | To select a component, use... |
| Using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select features and components, ordered selection of the features and components is required | * 1 to mark the direction axis * 4 to mark the features to pattern | * 1 to mark the components to pattern * 2 to mark the direction axis |
| Directly selecting a feature or axis using [IFeature::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~Select2.html) | * 1 to mark the direction axis * 4 to mark the features to pattern | [ISelectData::Mark](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData~Mark.html) and [Component2::Select3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select3.html)   * 1 to mark the components to pattern * 2 to mark the direction axis |

If VaryInstance = true, then to indicate how to vary the individual pattern instances, decide on the type of pattern and call its corresponding method before calling this method:

| Type... | Method... |
| --- | --- |
| Increment | [IFeatureManager::InsertVaryInstanceIncrement](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertVaryInstanceIncrement.html) |
| Override | [IFeatureManager::InsertVaryInstanceOverride](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertVaryInstanceOverride.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ICircularPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICircularPatternFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0