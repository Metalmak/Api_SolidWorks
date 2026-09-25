<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCircularPattern5.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureCircularPattern5 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureCircularPattern5 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Number*
:   Number of instances of the circular pattern to insert in Direction 1, including the original instance

*Spacing*
:   Spacing between each instance in Direction 1 of the circular pattern or, if EqualSpacing is true, then the total angle in radians

*FlipDirection*
:   True to flip the direction of the circular pattern in Direction 1, false to not

*DName*
:   Name of the angular dimension defining Direction 1 of the pattern

*GeometryPattern*
:   True to use geometry pattern, false to not

*EqualSpacing*
:   True to use equal spacing in Direction 1, false to not

*VaryInstance*
:   True to vary the dimensions or spacing of individual pattern instances, false to not; valid only if GeometryPattern = false (see **Remarks**)

*SyncSubAssemblies*
:   True to move components in the patterned instances when components are moved in the seed flexible subassembly, false to not

*BDir2*
:   True to create a bidirectional circular pattern feature, false to not

*BSymmetric*
:   True to create a symmetric circular pattern feature in Direction 2, false to create an asymmetrical circular pattern feature in Direction 2; valid only if BDir2 is true

*Number2*
:   Number of instances to insert in Direction 2; valid only if BDir2 is true

*Spacing2*
:   Distance between pattern instances in Direction 2; valid only if BDir2 is true

*DName2*
:   Name of the angular dimension defining Direction 2 of the pattern; valid only if BDir2 is true

*EqualSpacing2*
:   True to use equal spacing in Direction 2, false to not; valid only if BDir2 is true and BSymmetric is false

Obsolete. See [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) and the Remarks in [ICircularPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICircularPatternFeatureData.html) and [ILocalCircularPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureCircularPattern5( _    ByVal Number As System.Integer, _    ByVal Spacing As System.Double, _    ByVal FlipDirection As System.Boolean, _    ByVal DName As System.String, _    ByVal GeometryPattern As System.Boolean, _    ByVal EqualSpacing As System.Boolean, _    ByVal VaryInstance As System.Boolean, _    ByVal SyncSubAssemblies As System.Boolean, _    ByVal BDir2 As System.Boolean, _    ByVal BSymmetric As System.Boolean, _    ByVal Number2 As System.Integer, _    ByVal Spacing2 As System.Double, _    ByVal DName2 As System.String, _    ByVal EqualSpacing2 As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Number As System.Integer Dim Spacing As System.Double Dim FlipDirection As System.Boolean Dim DName As System.String Dim GeometryPattern As System.Boolean Dim EqualSpacing As System.Boolean Dim VaryInstance As System.Boolean Dim SyncSubAssemblies As System.Boolean Dim BDir2 As System.Boolean Dim BSymmetric As System.Boolean Dim Number2 As System.Integer Dim Spacing2 As System.Double Dim DName2 As System.String Dim EqualSpacing2 As System.Boolean Dim value As Feature   value = instance.FeatureCircularPattern5(Number, Spacing, FlipDirection, DName, GeometryPattern, EqualSpacing, VaryInstance, SyncSubAssemblies, BDir2, BSymmetric, Number2, Spacing2, DName2, EqualSpacing2) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureCircularPattern5(     System.int Number,    System.double Spacing,    System.bool FlipDirection,    System.string DName,    System.bool GeometryPattern,    System.bool EqualSpacing,    System.bool VaryInstance,    System.bool SyncSubAssemblies,    System.bool BDir2,    System.bool BSymmetric,    System.int Number2,    System.double Spacing2,    System.string DName2,    System.bool EqualSpacing2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureCircularPattern5(  &   System.int Number, &   System.double Spacing, &   System.bool FlipDirection, &   System.String^ DName, &   System.bool GeometryPattern, &   System.bool EqualSpacing, &   System.bool VaryInstance, &   System.bool SyncSubAssemblies, &   System.bool BDir2, &   System.bool BSymmetric, &   System.int Number2, &   System.double Spacing2, &   System.String^ DName2, &   System.bool EqualSpacing2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Number*
:   Number of instances of the circular pattern to insert in Direction 1, including the original instance

*Spacing*
:   Spacing between each instance in Direction 1 of the circular pattern or, if EqualSpacing is true, then the total angle in radians

*FlipDirection*
:   True to flip the direction of the circular pattern in Direction 1, false to not

*DName*
:   Name of the angular dimension defining Direction 1 of the pattern

*GeometryPattern*
:   True to use geometry pattern, false to not

*EqualSpacing*
:   True to use equal spacing in Direction 1, false to not

*VaryInstance*
:   True to vary the dimensions or spacing of individual pattern instances, false to not; valid only if GeometryPattern = false (see **Remarks**)

*SyncSubAssemblies*
:   True to move components in the patterned instances when components are moved in the seed flexible subassembly, false to not

*BDir2*
:   True to create a bidirectional circular pattern feature, false to not

*BSymmetric*
:   True to create a symmetric circular pattern feature in Direction 2, false to create an asymmetrical circular pattern feature in Direction 2; valid only if BDir2 is true

*Number2*
:   Number of instances to insert in Direction 2; valid only if BDir2 is true

*Spacing2*
:   Distance between pattern instances in Direction 2; valid only if BDir2 is true

*DName2*
:   Name of the angular dimension defining Direction 2 of the pattern; valid only if BDir2 is true

*EqualSpacing2*
:   True to use equal spacing in Direction 2, false to not; valid only if BDir2 is true and BSymmetric is false

#### Return Value

Circular pattern [feature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureCircularPattern5.

# ![](dotnetimages/collapse.gif)Remarks

| If... | To select a feature, use... | To select a component, use... |
| --- | --- | --- |
| Using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select features and components, ordered selection of the features and components is required | * 1 to mark the direction axis * 4 to mark the features to pattern | * 1 to mark the components to pattern * 2 to mark the direction axis |
| Directly selecting a feature or axis using [IFeature::Select2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~Select2.html) | * 1 to mark the direction axis * 4 to mark the features to pattern | [ISelectData::Mark](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData~Mark.html) and [Component2::Select3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select3.html)   * 1 to mark the components to pattern * 2 to mark the direction axis |

If VaryInstance = true, then to indicate how to vary the individual pattern instances, decide on the type of pattern and call its corresponding method before calling this method:

| Type | Method |
| --- | --- |
| Increment | [IFeatureManager::InsertVaryInstanceIncrement](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertVaryInstanceIncrement.html) |
| Override | [IFeatureManager::InsertVaryInstanceOverride](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertVaryInstanceOverride.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0