<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager~CreateNewStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateNewStudy Method (ICWStudyManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) : CreateNewStudy Method (ICWStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   New study name

*NAnalysisType*
:   Type of study as defined in [swsAnalysisStudyType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAnalysisStudyType_e.html)

*NMeshType*
:   Mesh type as defined in [swsMeshType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshType_e.html) (see **Remarks**)

*Errors*
:   Error as defined in [swsStudyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyError_e.html)

Obsolete. Superseded by [ICWStudyManager::CreateNewStudy2.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudyManager~CreateNewStudy2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateNewStudy( _    ByVal SName As System.String, _    ByVal NAnalysisType As System.Integer, _    ByVal NMeshType As System.Integer, _    ByRef Errors As System.Integer _ ) As CWStudy ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyManager Dim SName As System.String Dim NAnalysisType As System.Integer Dim NMeshType As System.Integer Dim Errors As System.Integer Dim value As CWStudy   value = instance.CreateNewStudy(SName, NAnalysisType, NMeshType, Errors) ``` | |

| C# |  |
| --- | --- |
| ``` CWStudy CreateNewStudy(     System.string SName,    System.int NAnalysisType,    System.int NMeshType,    out System.int Errors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWStudy^ CreateNewStudy(  &   System.String^ SName, &   System.int NAnalysisType, &   System.int NMeshType, &   [Out] System.int Errors ) ``` | |

#### Parameters

*SName*
:   New study name

*NAnalysisType*
:   Type of study as defined in [swsAnalysisStudyType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsAnalysisStudyType_e.html)

*NMeshType*
:   Mesh type as defined in [swsMeshType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshType_e.html) (see **Remarks**)

*Errors*
:   Error as defined in [swsStudyError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyError_e.html)

#### Return Value

[Study](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudy.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyManager::CreateNewStudy.

# ![](dotnetimages/collapse.gif)Example

[Create Nonlinear Study and Apply Materials (C#)](Create_Nonlinear_Study_and_Apply_Materials_Example_CSharp.htm)

[Create Nonlinear Study and Apply Materials (VB.NET)](Create_Nonlinear_Study_and_Apply_Materials_Example_VBNET.htm)

[Create Nonlinear Study and Apply Materials (VBA)](Create_Nonlinear_Study_and_Apply_Materials_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Valid mesh types for different types of studies:

|  |  |  |  |  |
| --- | --- | --- | --- | --- |
| Study Type | Solid Mesh | Shell Mesh | Mixed Mesh (Solid & Shell) | Beam Mesh |
| Static | Supported | Supported | Supported | Supported |
| Frequency | Supported | Supported | Supported | Supported |
| Buckling | Supported | Supported | Supported | Supported |
| Thermal | Supported | Supported | Supported | Supported |
| Nonlinear | Supported | Supported | Supported | Not Supported |
| Linear Dynamic | Supported | Supported | Supported | Not Supported |
| Drop Test | Supported | Not Supported | Not Supported | Not Supported |
| Fatigue | Not Applicable | Not Applicable | Not Applicable | Not Applicable |
| Optimization | Not Applicable | Not Applicable | Not Applicable | Not Applicable |

**NOTES:**

* For documents with surface geometry only (no solids), only RefSurfShellElementMesh is supported.

  * BeamElementMesh is supported only for static, buckling, and frequency studies.

    * Drop test studies support solid mesh only.

      * For optimization and fatigue studies do not have mesh on their own. They use mesh of referenced studies. Mesh type is set to SolidElementMesh.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html)

[ICWStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0