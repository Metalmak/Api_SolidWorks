<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindTouchingEdgeFacePairs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| FindTouchingEdgeFacePairs Method (ICWContactManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) : FindTouchingEdgeFacePairs Method (ICWContactManager) |

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

*NEdgeFaces*
:   Number of touching shell edges and faces

Finds touching shell edges and faces in the specified bodies or components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FindTouchingEdgeFacePairs( _    ByVal VarCompBodies As System.Object, _    ByRef NEdgeFaces As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactManager Dim VarCompBodies As System.Object Dim NEdgeFaces As System.Integer Dim value As System.Object   value = instance.FindTouchingEdgeFacePairs(VarCompBodies, NEdgeFaces) ``` | |

| C# |  |
| --- | --- |
| ``` System.object FindTouchingEdgeFacePairs(     System.object VarCompBodies,    out System.int NEdgeFaces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ FindTouchingEdgeFacePairs(  &   System.Object^ VarCompBodies, &   [Out] System.int NEdgeFaces ) ``` | |

#### Parameters

*VarCompBodies*
:   Array of bodies or components

*NEdgeFaces*
:   Number of touching shell edges and faces

#### Return Value

Array of touching shell edge and face pairs

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactManager::FindTouchingEdgeFacePairs.

# ![](dotnetimages/collapse.gif)Remarks

NEdgeFaces contains the size of the returned array. The returned array contains consecutive pairs of touching entities.

To create contact sets using the returned array, call [ICWContactManager::CreateContactSetsFromPairList](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactSetsFromPairList.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html)

[ICWContactManager::FindNonTouchingPairs Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindNonTouchingPairs.html)

[ICWContactManager::FindTouchingFacePairs Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindTouchingFacePairs.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0