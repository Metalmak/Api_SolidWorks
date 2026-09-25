<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~GetPoorMeshQualityElementList2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPoorMeshQualityElementList2 Method (ICWMesh) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html) : GetPoorMeshQualityElementList2 Method (ICWMesh) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NMeshQualityKPI*
:   Mesh element quality criterion as defined in [swsMeshElementQualityKPI\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshElementQualityKPI_e.html) (see **Remarks**)

*DLimitVal*
:   Upper or lower limit of NMeshQualityKPI, beyond which the mesh becomes poor quality (see **Remarks**)

*NJacobianPts*
:   Jacobian points criterion (see **Remarks**)

*BCreateplot*
:   -1 or true to create a plot, 0 or false to not

*VarElementIDs*
:   Array of element IDs

*ErrorCode*
:   Error code as defined by [swsMeshKPIErrCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshKPIErrCode_e.html)

Gets the Mesh Quality Diagnostics element list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPoorMeshQualityElementList2( _    ByVal NMeshQualityKPI As System.Integer, _    ByVal DLimitVal As System.Double, _    ByVal NJacobianPts As System.Integer, _    ByVal BCreateplot As System.Boolean, _    ByRef VarElementIDs As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMesh Dim NMeshQualityKPI As System.Integer Dim DLimitVal As System.Double Dim NJacobianPts As System.Integer Dim BCreateplot As System.Boolean Dim VarElementIDs As System.Object Dim ErrorCode As System.Integer Dim value As System.Integer   value = instance.GetPoorMeshQualityElementList2(NMeshQualityKPI, DLimitVal, NJacobianPts, BCreateplot, VarElementIDs, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetPoorMeshQualityElementList2(     System.int NMeshQualityKPI,    System.double DLimitVal,    System.int NJacobianPts,    System.bool BCreateplot,    out System.object VarElementIDs,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetPoorMeshQualityElementList2(  &   System.int NMeshQualityKPI, &   System.double DLimitVal, &   System.int NJacobianPts, &   System.bool BCreateplot, &   [Out] System.Object^ VarElementIDs, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NMeshQualityKPI*
:   Mesh element quality criterion as defined in [swsMeshElementQualityKPI\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshElementQualityKPI_e.html) (see **Remarks**)

*DLimitVal*
:   Upper or lower limit of NMeshQualityKPI, beyond which the mesh becomes poor quality (see **Remarks**)

*NJacobianPts*
:   Jacobian points criterion (see **Remarks**)

*BCreateplot*
:   -1 or true to create a plot, 0 or false to not

*VarElementIDs*
:   Array of element IDs

*ErrorCode*
:   Error code as defined by [swsMeshKPIErrCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMeshKPIErrCode_e.html)

#### Return Value

Number of elements in VarElementIDs

# ![](dotnetimages/collapse.gif)Remarks

This method:

* Corresponds to the Mesh Quality Diagnostics tool in SOLIDWORKS Simulation. Access the Mesh Quality Diagnostics PropertyManager in a SOLIDWORKS Simulation study by right-clicking **Mesh** in the study's FeatureManager design tree and selecting **Mesh Quality Diagnostics**.* Retrieves the IDs of elements satisfying the criterion specified by NMeshQualityKPI, DLimitVal, and NJacobianPts if valid.

If NMeshQualityKPI is swsMeshElementQualityKPI\_e.swsMeshElementQualityKPI\_:

* Volume or Area, then mesh has poor quality if less than DLimitVal; use NJacobianPts to specify the Jacobian points criterion.* AspectRatio or JacobianRatio or ElemSkewRatio, then mesh has poor quality if greater than DLimitVal. NJacobianPts is ignored.* JacobianRatio, then mesh has poor quality if greater than DLimitVal; use NJacobianPts to specify the Jacobian points criterion.

Possible values for NJacobianPts:

* 4  = Number of points inside the element tetrahedron near its vertices* 16 = Number of points inside the element tetrahedron* 29 = Number of points inside the element tetrahedron (same as 16 but calculates a more precise Jacobian ratio)* 10 = At nodes;  Number of points = 4 vertices + 6 midpoints on 6 edges of the element tetrahedron

For more information, read the **Simulation > Meshing > Mesh Quality Checks > Defining a Mesh Quality Plot** topic in the SOLIDWORKS Help.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMesh Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh.html)

[ICWMesh Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30