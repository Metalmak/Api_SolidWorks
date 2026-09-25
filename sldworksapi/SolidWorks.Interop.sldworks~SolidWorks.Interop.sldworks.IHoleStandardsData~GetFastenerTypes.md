<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTypes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFastenerTypes Method (IHoleStandardsData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) : GetFastenerTypes Method (IHoleStandardsData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StandardName*
:   Standard name (see **Remarks**)

*FastenerIndexes*
:   Array of fastener indexes

*FastenerNames*
:   Array of fastener names

Gets the fasteners in the specified Hole Wizard standard.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFastenerTypes( _    ByVal StandardName As System.String, _    ByRef FastenerIndexes As System.Object, _    ByRef FastenerNames As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleStandardsData Dim StandardName As System.String Dim FastenerIndexes As System.Object Dim FastenerNames As System.Object Dim value As System.Boolean   value = instance.GetFastenerTypes(StandardName, FastenerIndexes, FastenerNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetFastenerTypes(     System.string StandardName,    out System.object FastenerIndexes,    out System.object FastenerNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetFastenerTypes(  &   System.String^ StandardName, &   [Out] System.Object^ FastenerIndexes, &   [Out] System.Object^ FastenerNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StandardName*
:   Standard name (see **Remarks**)

*FastenerIndexes*
:   Array of fastener indexes

*FastenerNames*
:   Array of fastener names

#### Return Value

True if fastener types successfully retrieved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleStandardsData::GetFastenerTypes.

# ![](dotnetimages/collapse.gif)Example

See the [IHoleStandardsData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

To set StandardName, use [IHoleStandardsData::GetHoleStandards](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetHoleStandards.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html)

[IHoleStandardsData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0