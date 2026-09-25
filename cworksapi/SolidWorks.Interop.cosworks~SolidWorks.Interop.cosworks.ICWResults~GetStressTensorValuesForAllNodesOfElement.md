<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStressTensorValuesForAllNodesOfElement.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetStressTensorValuesForAllNodesOfElement Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetStressTensorValuesForAllNodesOfElement Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ElementNumbers*
:   An array of mesh element numbers for which to return nodal results; specify the element number of a single element (see Remarks)

*NUnits*
:   Units as defined in [swsStrengthUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrengthUnit_e.html)

*NStepNum*
:   Solution step number (use 1 for steady state)

*ErrorCode*
:   Error as defined in [swsNodalResultsOfElementError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsNodalResultsOfElementError_e.html)

Gets the stress tensor values for all nodes of the specified mesh elements at the specified solution step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetStressTensorValuesForAllNodesOfElement( _    ByVal ElementNumbers As System.Object, _    ByVal NUnits As System.Integer, _    ByVal NStepNum As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim ElementNumbers As System.Object Dim NUnits As System.Integer Dim NStepNum As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetStressTensorValuesForAllNodesOfElement(ElementNumbers, NUnits, NStepNum, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetStressTensorValuesForAllNodesOfElement(     System.object ElementNumbers,    System.int NUnits,    System.int NStepNum,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetStressTensorValuesForAllNodesOfElement(  &   System.Object^ ElementNumbers, &   System.int NUnits, &   System.int NStepNum, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ElementNumbers*
:   An array of mesh element numbers for which to return nodal results; specify the element number of a single element (see Remarks)

*NUnits*
:   Units as defined in [swsStrengthUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrengthUnit_e.html)

*NStepNum*
:   Solution step number (use 1 for steady state)

*ErrorCode*
:   Error as defined in [swsNodalResultsOfElementError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsNodalResultsOfElementError_e.html)

#### Return Value

Two-dimensional array of tensor stress values (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetStressTensorValuesForAllNodesOfElement.

# ![](dotnetimages/collapse.gif)Example

[Get Stress Tensor Values For Mesh (VBA)](Get_Stress_Tensor_Values_for_Mesh_Example_VB.htm)

[Get Stress Tensor Values For Mesh (VB.NET)](Get_Stress_Tensor_Values_For_Mesh_Example_VBNET.htm)

[Get Stress Tensor Values For Mesh (C#)](Get_Stress_Tensor_Values_For_Mesh_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for solid and shell meshes. Beam meshes are not supported.

Call [ICWMesh::ElementCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMesh~ElementCount.html) to specify ElementNumbers.

The number of rows in the returned two-dimensional array is:

```
    (n * m * p)
```

where:

* *n* = # elements in the mesh* *m* = # nodes for each element* *p =* 2 for shell meshes (top and bottom faces); 1 for solid meshes

Each row contains nine values:

```
    element_i, shell_face_i, node_i, tensor_value_1, tensor_value_2, tensor_value_3, tensor_value_4, tensor_value_5, tensor_value_6
```

where:

* *element\_i* = the zero-based index of the element in the mesh* *shell\_face\_i* = 0 for the top face of a shell mesh, 1 for the bottom face of a shell mesh, and -1 for a solid mesh* *node\_i* = the zero-based index of the node for this row's element

Therefore, the array returned for a shell mesh contains 18\**n*\**m* values in the following order:

```
[
```

```
   element_1, shell_face_0, node_1, tensor_value_1, tensor_value_2, tensor_value_3, tensor_value_4, tensor_value_5, tensor_value_6
```

```
   element_1, shell_face_0, node_2, tensor_value_1, tensor_value_2, tensor_value_3, tensor_value_4, tensor_value_5, tensor_value_6
```

```
   ...
```

```
   element_1, shell_face_0, node_m, tensor_value_1, tensor_value_2, tensor_value_3, tensor_value_4, tensor_value_5, tensor_value_6
```

```
   (repeat above for shell_face_1)
```

```
   (repeat above for element_2 through element_n)
```

```
]
```

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetStressForEntities3 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStressForEntities3.html)

[ICWResults::GetStressComponentForAllStepsAtNode Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStressComponentForAllStepsAtNode.html)

[ICWResults::GetStress Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetStress.html)

[ICWResults::GetMinMaxStress Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxStress.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP05