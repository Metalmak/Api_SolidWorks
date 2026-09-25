<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMateReference2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMateReference2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMateReference2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BstrMateReferenceName*
:   Name of mate reference

*PrimaryReferenceEntity*
:   Pointer to the primary mate, the [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*PrimaryReferenceType*
:   Primary mate's reference type as defined by swMateReferenceType\_e

*PrimaryReferenceAlignment*
:   Primary mate's reference alignment type as defined swMateReferenceAlignment\_e

*PrimaryReferenceAlignAxes*
:   True to align with the axes of the coordinate system or origin when forming a mate, false to not

*SecondaryReferenceEntity*
:   Pointer to the secondary mate, the [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*SecondaryReferenceType*
:   Secondary mate's reference type as defined by swMateReferenceType\_e

*SecondaryReferenceAlignment*
:   Secondary mate's alignment type as defined swMateReferenceAlignment\_e

*SecondaryReferenceAlignAxes*
:   True to align with the axes of the coordinate system or origin when forming a mate, false to not

*TertiaryReferenceEntity*
:   Pointer to the tertiary mate, the [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*TertiaryReferenceType*
:   Tertiary mate's reference type as defined by swMateReferenceType\_e

*TertiaryReferenceAlignment*
:   Tertiary mate's reference alignment as defined by swMateReferenceAlignment\_e

Inserts a mate reference for a part or assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMateReference2( _    ByVal BstrMateReferenceName As System.String, _    ByVal PrimaryReferenceEntity As Entity, _    ByVal PrimaryReferenceType As System.Integer, _    ByVal PrimaryReferenceAlignment As System.Integer, _    ByVal PrimaryReferenceAlignAxes As System.Boolean, _    ByVal SecondaryReferenceEntity As Entity, _    ByVal SecondaryReferenceType As System.Integer, _    ByVal SecondaryReferenceAlignment As System.Integer, _    ByVal SecondaryReferenceAlignAxes As System.Boolean, _    ByVal TertiaryReferenceEntity As Entity, _    ByVal TertiaryReferenceType As System.Integer, _    ByVal TertiaryReferenceAlignment As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BstrMateReferenceName As System.String Dim PrimaryReferenceEntity As Entity Dim PrimaryReferenceType As System.Integer Dim PrimaryReferenceAlignment As System.Integer Dim PrimaryReferenceAlignAxes As System.Boolean Dim SecondaryReferenceEntity As Entity Dim SecondaryReferenceType As System.Integer Dim SecondaryReferenceAlignment As System.Integer Dim SecondaryReferenceAlignAxes As System.Boolean Dim TertiaryReferenceEntity As Entity Dim TertiaryReferenceType As System.Integer Dim TertiaryReferenceAlignment As System.Integer Dim value As Feature   value = instance.InsertMateReference2(BstrMateReferenceName, PrimaryReferenceEntity, PrimaryReferenceType, PrimaryReferenceAlignment, PrimaryReferenceAlignAxes, SecondaryReferenceEntity, SecondaryReferenceType, SecondaryReferenceAlignment, SecondaryReferenceAlignAxes, TertiaryReferenceEntity, TertiaryReferenceType, TertiaryReferenceAlignment) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMateReference2(     System.string BstrMateReferenceName,    Entity PrimaryReferenceEntity,    System.int PrimaryReferenceType,    System.int PrimaryReferenceAlignment,    System.bool PrimaryReferenceAlignAxes,    Entity SecondaryReferenceEntity,    System.int SecondaryReferenceType,    System.int SecondaryReferenceAlignment,    System.bool SecondaryReferenceAlignAxes,    Entity TertiaryReferenceEntity,    System.int TertiaryReferenceType,    System.int TertiaryReferenceAlignment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMateReference2(  &   System.String^ BstrMateReferenceName, &   Entity^ PrimaryReferenceEntity, &   System.int PrimaryReferenceType, &   System.int PrimaryReferenceAlignment, &   System.bool PrimaryReferenceAlignAxes, &   Entity^ SecondaryReferenceEntity, &   System.int SecondaryReferenceType, &   System.int SecondaryReferenceAlignment, &   System.bool SecondaryReferenceAlignAxes, &   Entity^ TertiaryReferenceEntity, &   System.int TertiaryReferenceType, &   System.int TertiaryReferenceAlignment ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BstrMateReferenceName*
:   Name of mate reference

*PrimaryReferenceEntity*
:   Pointer to the primary mate, the [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*PrimaryReferenceType*
:   Primary mate's reference type as defined by swMateReferenceType\_e

*PrimaryReferenceAlignment*
:   Primary mate's reference alignment type as defined swMateReferenceAlignment\_e

*PrimaryReferenceAlignAxes*
:   True to align with the axes of the coordinate system or origin when forming a mate, false to not

*SecondaryReferenceEntity*
:   Pointer to the secondary mate, the [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*SecondaryReferenceType*
:   Secondary mate's reference type as defined by swMateReferenceType\_e

*SecondaryReferenceAlignment*
:   Secondary mate's alignment type as defined swMateReferenceAlignment\_e

*SecondaryReferenceAlignAxes*
:   True to align with the axes of the coordinate system or origin when forming a mate, false to not

*TertiaryReferenceEntity*
:   Pointer to the tertiary mate, the [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*TertiaryReferenceType*
:   Tertiary mate's reference type as defined by swMateReferenceType\_e

*TertiaryReferenceAlignment*
:   Tertiary mate's reference alignment as defined by swMateReferenceAlignment\_e

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMateReference2.

# ![](dotnetimages/collapse.gif)Example

[Edit Mate Reference (C#)](Edit_Mate_Reference_Example_CSharp.htm)

[Edit Mate Reference (VB.NET)](Edit_Mate_Reference_Example_VBNET.htm)

[Edit Mate Reference (VBA)](Edit_Mate_Reference_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IMateReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0