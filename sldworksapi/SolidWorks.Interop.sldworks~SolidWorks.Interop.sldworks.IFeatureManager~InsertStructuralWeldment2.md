<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertStructuralWeldment2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertStructuralWeldment2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertStructuralWeldment2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Path*
:   Path, filename, and name of the type of structural member to insert

*EndCond*
:   End condition as defined in swSolidworksWeldmentEndCondOptions\_e

*Angle*
:   Angle of rotation of the sketch about the sketch segment

*Merge*
:   True to merge the bodies of the arc segments to the adjacent bodies, false to not

Obsolete. Superseded by [IFeatureManager::InsertStructuralWeldment3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertStructuralWeldment3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertStructuralWeldment2( _    ByVal Path As System.String, _    ByVal EndCond As System.Integer, _    ByVal Angle As System.Double, _    ByVal Merge As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Path As System.String Dim EndCond As System.Integer Dim Angle As System.Double Dim Merge As System.Boolean Dim value As Feature   value = instance.InsertStructuralWeldment2(Path, EndCond, Angle, Merge) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertStructuralWeldment2(     System.string Path,    System.int EndCond,    System.double Angle,    System.bool Merge ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertStructuralWeldment2(  &   System.String^ Path, &   System.int EndCond, &   System.double Angle, &   System.bool Merge ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Path*
:   Path, filename, and name of the type of structural member to insert

*EndCond*
:   End condition as defined in swSolidworksWeldmentEndCondOptions\_e

*Angle*
:   Angle of rotation of the sketch about the sketch segment

*Merge*
:   True to merge the bodies of the arc segments to the adjacent bodies, false to not

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertStructuralWeldment2.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IStructuralMemberFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStructuralMemberFeatureData.html)

[IFeatureManager::InsertStructuralWeldment3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertStructuralWeldment3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0