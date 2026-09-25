<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditConcentricMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditConcentricMate Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : EditConcentricMate Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AlignFromEnum*
:   Type of mate alignment as defined in swMateAlign\_e

*ConcentricPositionType*
:   Misaligned concentric mate position as defined in swConcentricAlignmentType\_e

*ConcentricToleranceCheck*
:   True to override the deviation, false to have SOLIDWORKS calculate the deviation

*ConcentricToleranceValue*
:   Maximum deviation; valid only when ConcentricToleranceCheck is true

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

Edits a misaligned concentric mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub EditConcentricMate( _    ByVal AlignFromEnum As System.Integer, _    ByVal ConcentricPositionType As System.Integer, _    ByVal ConcentricToleranceCheck As System.Boolean, _    ByVal ConcentricToleranceValue As System.Double, _    ByRef ErrorStatus As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim AlignFromEnum As System.Integer Dim ConcentricPositionType As System.Integer Dim ConcentricToleranceCheck As System.Boolean Dim ConcentricToleranceValue As System.Double Dim ErrorStatus As System.Integer   instance.EditConcentricMate(AlignFromEnum, ConcentricPositionType, ConcentricToleranceCheck, ConcentricToleranceValue, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` void EditConcentricMate(     System.int AlignFromEnum,    System.int ConcentricPositionType,    System.bool ConcentricToleranceCheck,    System.double ConcentricToleranceValue,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void EditConcentricMate(  &   System.int AlignFromEnum, &   System.int ConcentricPositionType, &   System.bool ConcentricToleranceCheck, &   System.double ConcentricToleranceValue, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AlignFromEnum*
:   Type of mate alignment as defined in swMateAlign\_e

*ConcentricPositionType*
:   Misaligned concentric mate position as defined in swConcentricAlignmentType\_e

*ConcentricToleranceCheck*
:   True to override the deviation, false to have SOLIDWORKS calculate the deviation

*ConcentricToleranceValue*
:   Maximum deviation; valid only when ConcentricToleranceCheck is true

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::EditConcentricMate.

# ![](dotnetimages/collapse.gif)Example

See the [IAssemblyDoc::AddConcentricMateWithTolerance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddConcentricMateWithTolerance.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Select these entities before calling this method:

* Two entities that define the misaligned concentric mate* Misaligned concentric mate

A parent non-misaligned (i.e., standard) concentric mate must already exist for the selected misaligned concentric mate. If a suitable parent concentric mate does not exist, then the selected misaligned concentric mate changes to a standard concentric mate. You can also change a misaligned concentric mate to a standard concentric mate using [IAssemblyDoc::EditMate4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditMate4.html).

After calling IAssemblyDoc::EditConcentricMate, call [IModelDoc2::EditRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRebuild3.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddConcentricMateWithTolerance Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddConcentricMateWithTolerance.html)

[IAssemblyDoc::AddMate5 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0