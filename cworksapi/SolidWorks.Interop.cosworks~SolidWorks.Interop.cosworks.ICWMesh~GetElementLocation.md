<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetElementLocation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetElementLocation Method (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetElementLocation Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NNodeNo*
:   Element number

*XVal*
:   X coordinate of the element's center

*YVal*
:   Y coordinate of the element's center

*ZVal*
:   Z coordinate of the element's center

Gets the coordinates of an element's center.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetElementLocation( _    ByVal NNodeNo As System.Integer, _    ByRef XVal As System.Double, _    ByRef YVal As System.Double, _    ByRef ZVal As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim NNodeNo As System.Integer Dim XVal As System.Double Dim YVal As System.Double Dim ZVal As System.Double Dim value As System.Integer   value = instance.GetElementLocation(NNodeNo, XVal, YVal, ZVal) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetElementLocation(     System.int NNodeNo,    out System.double XVal,    out System.double YVal,    out System.double ZVal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetElementLocation(  &   System.int NNodeNo, &   [Out] System.double XVal, &   [Out] System.double YVal, &   [Out] System.double ZVal ) ``` | |

#### Parameters

*NNodeNo*
:   Element number

*XVal*
:   X coordinate of the element's center

*YVal*
:   Y coordinate of the element's center

*ZVal*
:   Z coordinate of the element's center

#### Return Value

Error as defined in [swsMeshElementNodeLocation\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshElementNodeLocation_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMesh::GetElementLocation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

[ICWMesh::GetDefaultElementSizeAndTolerance Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetDefaultElementSizeAndTolerance.html)

[ICWMesh::GetElementDataFromEntity Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetElementDataFromEntity.html)

[ICWMesh::GetElements Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetElements.html)

[ICWMesh::ElementCount Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ElementCount.html)

[ICWMesh::ElementSize Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ElementSize.html)

[ICWMesh::MinElementsInCircle Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MinElementsInCircle.html)

[ICWMesh::MaxAspectRatio Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~MaxAspectRatio.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0