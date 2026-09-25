<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddConcentricMateWithTolerance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddConcentricMateWithTolerance Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddConcentricMateWithTolerance Method (IAssemblyDoc) |

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

Adds a misaligned concentric mate to this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddConcentricMateWithTolerance( _    ByVal AlignFromEnum As System.Integer, _    ByVal ConcentricPositionType As System.Integer, _    ByVal ConcentricToleranceCheck As System.Boolean, _    ByVal ConcentricToleranceValue As System.Double, _    ByRef ErrorStatus As System.Integer _ ) As Mate2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim AlignFromEnum As System.Integer Dim ConcentricPositionType As System.Integer Dim ConcentricToleranceCheck As System.Boolean Dim ConcentricToleranceValue As System.Double Dim ErrorStatus As System.Integer Dim value As Mate2   value = instance.AddConcentricMateWithTolerance(AlignFromEnum, ConcentricPositionType, ConcentricToleranceCheck, ConcentricToleranceValue, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` Mate2 AddConcentricMateWithTolerance(     System.int AlignFromEnum,    System.int ConcentricPositionType,    System.bool ConcentricToleranceCheck,    System.double ConcentricToleranceValue,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Mate2^ AddConcentricMateWithTolerance(  &   System.int AlignFromEnum, &   System.int ConcentricPositionType, &   System.bool ConcentricToleranceCheck, &   System.double ConcentricToleranceValue, &   [Out] System.int ErrorStatus ) ``` | |

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

#### Return Value

Misaligned concentric [mate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddConcentricMateWithTolerance.

# ![](dotnetimages/collapse.gif)Example

[Add and Edit Misaligned Symmetric Concentric Mate (VBA)](Add_and_Edit_Misaligned_Symmetric_Concentric_Mate_Example_VB.htm)

[Add and Edit Misaligned Symmetric Concentric Mate (VB.NET)](Add_and_Edit_Misaligned_Symmetric_Concentric_Mate_Example_VBNET.htm)

[Add and Edit Misaligned Symmetric Concentric Mate (C#)](Add_and_Edit_Misaligned_Symmetric_Concentric_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Select the two entities to mate before calling this method. A parent non-misaligned (i.e., standard) concentric mate must already exist between the selected entities. If a suitable parent concentric mate does not exist between the selected entities, then a standard concentric mate is created.

**NOTE:** The typical way to add a standard concentric mate is to use [IAssemblyDoc::AddMate5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate5.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::EditConcentricMate Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditConcentricMate.html)

[IAssemblyDoc::EditMate4 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditMate4.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0