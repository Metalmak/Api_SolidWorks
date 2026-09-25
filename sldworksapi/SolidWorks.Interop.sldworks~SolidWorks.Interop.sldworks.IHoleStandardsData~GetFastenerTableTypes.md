<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTableTypes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFastenerTableTypes Method (IHoleStandardsData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) : GetFastenerTableTypes Method (IHoleStandardsData) |

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

*FastenerID*
:   Fastener ID (see **Remarks**)

*FastenerTableTypeIDs*
:   Array of three fastener table type IDs (see **Remarks**)

Gets the array of three fastener table type IDs for the given fastener in the given Hole Wizard standard.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFastenerTableTypes( _    ByVal StandardName As System.String, _    ByVal FastenerID As System.Integer, _    ByRef FastenerTableTypeIDs As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleStandardsData Dim StandardName As System.String Dim FastenerID As System.Integer Dim FastenerTableTypeIDs As System.Object Dim value As System.Boolean   value = instance.GetFastenerTableTypes(StandardName, FastenerID, FastenerTableTypeIDs) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetFastenerTableTypes(     System.string StandardName,    System.int FastenerID,    out System.object FastenerTableTypeIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetFastenerTableTypes(  &   System.String^ StandardName, &   System.int FastenerID, &   [Out] System.Object^ FastenerTableTypeIDs ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StandardName*
:   Standard name (see **Remarks**)

*FastenerID*
:   Fastener ID (see **Remarks**)

*FastenerTableTypeIDs*
:   Array of three fastener table type IDs (see **Remarks**)

#### Return Value

True if the fastener table type IDs are successfully retrieved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleStandardsData::GetFastenerTableTypes.

# ![](dotnetimages/collapse.gif)Example

See the [IHoleStandardsData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

Each fastener in a given standard has three tables associated with it: size, thread data, and screw clearances. This method retrieves internal IDs of all three table types as defined in swFastenerTableTypes\_e for FastenerID in StandardName.

To set:

* StandardName, use [IHoleStandardsData::GetHoleStandards](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetHoleStandards.html).* FastenerID, use [IHoleStandardsData::GetFastenerTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTypes.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html)

[IHoleStandardsData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0