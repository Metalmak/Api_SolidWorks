<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinkageRodEndEditErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsLinkageRodEndEditErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsLinkageRodEndEditErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Linkage rod connector errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsLinkageRodEndEditErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsLinkageRodEndEditErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsLinkageRodEndEditErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsLinkageRodEndEditErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsLinkageRodErrCode\_InadequateEntitiesSelection** | 24 = Insufficient number of entities selected for a valid linkage rod connector |
| **swsLinkageRodErrCode\_InvalidArray** | 11 = Invalid array of section parameters |
| **swsLinkageRodErrCode\_InvalidCoAxialSelection** | 6 = Select non-co-axial concentric cylindrical faces or edges (for shells or surface bodies) at one end |
| **swsLinkageRodErrCode\_InvalidJointTypeSel** | 8 = Select a vertex that is not a pivot joint type |
| **swsLinkageRodErrCode\_InvalidLibraryMaterialDetails** | 19 = Invalid library path/name or non-available material name |
| **swsLinkageRodErrCode\_InvalidMass** | 23 |
| **swsLinkageRodErrCode\_InvalidMaterialSourceType** | 16 = Select material source type from swsMaterialSourceType\_e |
| **swsLinkageRodErrCode\_InvalidNonCoAxialSelection** | 5 = Select co-axial concentric cylindrical faces or edges (for shells or surface bodies) at one end |
| **swsLinkageRodErrCode\_InvalidNonConcentricSelection** | 7 = Select concentric cylindrical edges from shell or surface bodies |
| **swsLinkageRodErrCode\_InvalidParamDataType** | 13 = Use double section parameter for given section type |
| **swsLinkageRodErrCode\_InvalidParamsCount** | 12 = Invalid number of section parameters for given section type |
| **swsLinkageRodErrCode\_InvalidRodSectionType** | 10 = Select section type from swsCRSectionType\_e |
| **swsLinkageRodErrCode\_InvalidSelection** | 4 = Select cylindrical faces or a single vertex for solid bodies; select edges for shells or surface bodies |
| **swsLinkageRodErrCode\_InvalidUnitType** | 15 = Select unit type from swsUnit\_e |
| **swsLinkageRodErrCode\_NoActiveDoc** | 1 |
| **swsLinkageRodErrCode\_NoActiveStudy** | 2 |
| **swsLinkageRodErrCode\_OffsetOptionNotAvailable** | 9 = Offset direction and values not available for selected vertex |
| **swsLinkageRodErrCode\_OutOfRangePoissonRatio** | 21 = 0 < Poisson Ratio < 1 |
| **swsLinkageRodErrCode\_OutOfRangeThermalCoefficient** | 22 = 0 < Thermal Coefficient < 1e+16 |
| **swsLinkageRodErrCode\_OutOfRangeYoungsModulus** | 20 = 0 < Young's Modulus < 1e+16 |
| **swsLinkageRodErrCode\_SetLibraryMaterialNA** | 18 = Setting the library material is allowed only when Material Source Type = swsMaterial\_Library |
| **swsLinkageRodErrCode\_SetMaterialPropertyNA** | 17 = Setting material property is only allowed when Material Source Type = swsMaterial\_Custom |
| **swsLinkageRodErrCode\_SetOperationNotSupported** | 3 = Editing before calling BeginEdit not allowed |
| **swsLinkageRodErrCode\_Successful** | 0 |
| **swsLinkageRodErrCode\_ZeroParamValue** | 14 = Invalid section parameter value for given section type |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)