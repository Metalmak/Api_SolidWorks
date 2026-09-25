<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindNonTouchingPairs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| FindNonTouchingPairs Method (ICWContactManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) : FindNonTouchingPairs Method (ICWContactManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarCompBodies*
:   Array of bodies or components

*DMin*
:   Minimum clearance; face pairs closer than this distance do not appear in the returned array

*DMax*
:   Maximum clearance; face pairs further apart than this distance do not appear in the returned array

*NEnts*
:   Number of non-touching faces

Finds non-touching faces within the specified minimum and maximum distance in the specified bodies or components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FindNonTouchingPairs( _    ByVal VarCompBodies As System.Object, _    ByVal DMin As System.Double, _    ByVal DMax As System.Double, _    ByRef NEnts As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactManager Dim VarCompBodies As System.Object Dim DMin As System.Double Dim DMax As System.Double Dim NEnts As System.Integer Dim value As System.Object   value = instance.FindNonTouchingPairs(VarCompBodies, DMin, DMax, NEnts) ``` | |

| C# |  |
| --- | --- |
| ``` System.object FindNonTouchingPairs(     System.object VarCompBodies,    System.double DMin,    System.double DMax,    out System.int NEnts ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ FindNonTouchingPairs(  &   System.Object^ VarCompBodies, &   System.double DMin, &   System.double DMax, &   [Out] System.int NEnts ) ``` | |

#### Parameters

*VarCompBodies*
:   Array of bodies or components

*DMin*
:   Minimum clearance; face pairs closer than this distance do not appear in the returned array

*DMax*
:   Maximum clearance; face pairs further apart than this distance do not appear in the returned array

*NEnts*
:   Number of non-touching faces

#### Return Value

Array of non-touching face pairs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactManager::FindNonTouchingPairs.

# ![](dotnetimages/collapse.gif)Remarks

nEnts contains the size of the returned array. The returned array contains consecutive pairs of non-touching faces.

To create contact sets using the returned array, call [ICWContactManager::CreateContactSetsFromPairList](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactSetsFromPairList.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html)

[ICWContactManager::FindTouchingEdgeFacePairs Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindTouchingEdgeFacePairs.html)

[ICWContactManager::FindTouchingFacePairs Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindTouchingFacePairs.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0