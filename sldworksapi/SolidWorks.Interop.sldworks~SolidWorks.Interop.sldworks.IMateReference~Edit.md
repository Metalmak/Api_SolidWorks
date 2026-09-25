<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference~Edit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Edit Method (IMateReference) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMateReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference.html) : Edit Method (IMateReference) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BstrMateReferenceName*
:   Name of the new mate reference, which replaces the selected mate reference

*PrimaryReferenceEntity*
:   Primary mate reference entity, a pointer to an [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*PrimaryReferenceType*
:   Type of mate as defined by swMateReferenceType\_e for PrimaryReferenceEntity

*PrimaryReferenceAlignment*
:   Type of alignment as defined by swMateReferenceAlignment\_e for PrimaryReferenceEntity

*SecondaryReferenceEntity*
:   Secondary mate reference entity, a pointer to an [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*SecondaryReferenceType*
:   Type of mate as defined by swMateReferenceType\_e for SecondaryReferenceEntity

*SecondaryReferenceAlignment*
:   Type of alignment as defined by swMateReferenceAlignment\_e for SecondaryReferenceEntity

*TertiaryReferenceEntity*
:   Tertiary mate reference entity, a pointer to an [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*TertiaryReferenceType*
:   Type of mate as defined by swMateReferenceType\_e for TertiaryReferenceEntity

*TertiaryReferenceAlignment*
:   Type of alignment as defined by swMateReferenceAlignment\_e for TertiaryReferenceEntity

Lets you edit the selected mate reference.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Edit( _    ByVal BstrMateReferenceName As System.String, _    ByVal PrimaryReferenceEntity As Entity, _    ByVal PrimaryReferenceType As System.Integer, _    ByVal PrimaryReferenceAlignment As System.Integer, _    ByVal SecondaryReferenceEntity As Entity, _    ByVal SecondaryReferenceType As System.Integer, _    ByVal SecondaryReferenceAlignment As System.Integer, _    ByVal TertiaryReferenceEntity As Entity, _    ByVal TertiaryReferenceType As System.Integer, _    ByVal TertiaryReferenceAlignment As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMateReference Dim BstrMateReferenceName As System.String Dim PrimaryReferenceEntity As Entity Dim PrimaryReferenceType As System.Integer Dim PrimaryReferenceAlignment As System.Integer Dim SecondaryReferenceEntity As Entity Dim SecondaryReferenceType As System.Integer Dim SecondaryReferenceAlignment As System.Integer Dim TertiaryReferenceEntity As Entity Dim TertiaryReferenceType As System.Integer Dim TertiaryReferenceAlignment As System.Integer Dim value As System.Boolean   value = instance.Edit(BstrMateReferenceName, PrimaryReferenceEntity, PrimaryReferenceType, PrimaryReferenceAlignment, SecondaryReferenceEntity, SecondaryReferenceType, SecondaryReferenceAlignment, TertiaryReferenceEntity, TertiaryReferenceType, TertiaryReferenceAlignment) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Edit(     System.string BstrMateReferenceName,    Entity PrimaryReferenceEntity,    System.int PrimaryReferenceType,    System.int PrimaryReferenceAlignment,    Entity SecondaryReferenceEntity,    System.int SecondaryReferenceType,    System.int SecondaryReferenceAlignment,    Entity TertiaryReferenceEntity,    System.int TertiaryReferenceType,    System.int TertiaryReferenceAlignment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Edit(  &   System.String^ BstrMateReferenceName, &   Entity^ PrimaryReferenceEntity, &   System.int PrimaryReferenceType, &   System.int PrimaryReferenceAlignment, &   Entity^ SecondaryReferenceEntity, &   System.int SecondaryReferenceType, &   System.int SecondaryReferenceAlignment, &   Entity^ TertiaryReferenceEntity, &   System.int TertiaryReferenceType, &   System.int TertiaryReferenceAlignment ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BstrMateReferenceName*
:   Name of the new mate reference, which replaces the selected mate reference

*PrimaryReferenceEntity*
:   Primary mate reference entity, a pointer to an [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*PrimaryReferenceType*
:   Type of mate as defined by swMateReferenceType\_e for PrimaryReferenceEntity

*PrimaryReferenceAlignment*
:   Type of alignment as defined by swMateReferenceAlignment\_e for PrimaryReferenceEntity

*SecondaryReferenceEntity*
:   Secondary mate reference entity, a pointer to an [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*SecondaryReferenceType*
:   Type of mate as defined by swMateReferenceType\_e for SecondaryReferenceEntity

*SecondaryReferenceAlignment*
:   Type of alignment as defined by swMateReferenceAlignment\_e for SecondaryReferenceEntity

*TertiaryReferenceEntity*
:   Tertiary mate reference entity, a pointer to an [IEntity](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEntity.html) object

*TertiaryReferenceType*
:   Type of mate as defined by swMateReferenceType\_e for TertiaryReferenceEntity

*TertiaryReferenceAlignment*
:   Type of alignment as defined by swMateReferenceAlignment\_e for TertiaryReferenceEntity

#### Return Value

Always True

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MateReference::Edit.

# ![](dotnetimages/collapse.gif)Example

[Edit Mate Reference (C#)](Edit_Mate_Reference_Example_CSharp.htm)

[Edit Mate Reference (VB.NET)](Edit_Mate_Reference_Example_VBNET.htm)

[Edit Mate Reference (VBA)](Edit_Mate_Reference_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To clear the previous references, you can pass Nothing or null for the primary, secondary, or tertiary reference entities.

This method applies the parameters to the actual features. After calling this method, call [IModelDoc2::EditRebuild](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html) to rebuild the model, and then call [IModelDocExtension::NeedsRebuild](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~NeedsRebuild.html) to determine if the rebuild was successful.

# ![](dotnetimages/collapse.gif)See Also

####

[IMateReference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference.html)

[IMateReference Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateReference_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0