<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeLocation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetNodeLocation Method (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetNodeLocation Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NNodeNo*
:   Node number

*XVal*
:   X coordinate

*YVal*
:   Y coordinate

*ZVal*
:   Z coordinate

Gets the coordinates of the specified node.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNodeLocation( _    ByVal NNodeNo As System.Integer, _    ByRef XVal As System.Double, _    ByRef YVal As System.Double, _    ByRef ZVal As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim NNodeNo As System.Integer Dim XVal As System.Double Dim YVal As System.Double Dim ZVal As System.Double Dim value As System.Integer   value = instance.GetNodeLocation(NNodeNo, XVal, YVal, ZVal) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetNodeLocation(     System.int NNodeNo,    out System.double XVal,    out System.double YVal,    out System.double ZVal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetNodeLocation(  &   System.int NNodeNo, &   [Out] System.double XVal, &   [Out] System.double YVal, &   [Out] System.double ZVal ) ``` | |

#### Parameters

*NNodeNo*
:   Node number

*XVal*
:   X coordinate

*YVal*
:   Y coordinate

*ZVal*
:   Z coordinate

#### Return Value

Error as defined in [swsMeshControlError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshControlError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetNodeLocation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GetNodeDataFromEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodeDataFromEntity.html)

[ICWMesh::GetNodes Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetNodes.html)

[ICWMesh::NodeCount Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~NodeCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0