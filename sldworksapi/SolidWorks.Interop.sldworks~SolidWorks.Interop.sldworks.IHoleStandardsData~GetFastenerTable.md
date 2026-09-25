<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFastenerTable Method (IHoleStandardsData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) : GetFastenerTable Method (IHoleStandardsData) |

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

*TableID*
:   Fastener table type ID (see **Remarks**)

*HoleTable*
:   [IHoleDataTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable.html)

Gets the Hole Wizard fastener table for the specified Hole Wizard standard, fastener ID, and fastener table type ID.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFastenerTable( _    ByVal StandardName As System.String, _    ByVal FastenerID As System.Integer, _    ByVal TableID As System.Integer, _    ByRef HoleTable As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleStandardsData Dim StandardName As System.String Dim FastenerID As System.Integer Dim TableID As System.Integer Dim HoleTable As System.Object Dim value As System.Boolean   value = instance.GetFastenerTable(StandardName, FastenerID, TableID, HoleTable) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetFastenerTable(     System.string StandardName,    System.int FastenerID,    System.int TableID,    out System.object HoleTable ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetFastenerTable(  &   System.String^ StandardName, &   System.int FastenerID, &   System.int TableID, &   [Out] System.Object^ HoleTable ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StandardName*
:   Standard name (see **Remarks**)

*FastenerID*
:   Fastener ID (see **Remarks**)

*TableID*
:   Fastener table type ID (see **Remarks**)

*HoleTable*
:   [IHoleDataTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleDataTable.html)

#### Return Value

True if fastener data table successfully retrieved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleStandardsData::GetFastenerTable.

# ![](dotnetimages/collapse.gif)Example

See the [IHoleStandardsData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

To set:

* StandardName, use [IHoleStandardsData::GetHoleStandards](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetHoleStandards.html).* FastenerID, use [IHoleStandardsData::GetFastenerTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTypes.html).* TableID, use [IHoleStandardsData::GetFastenerTableTypes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData~GetFastenerTableTypes.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleStandardsData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData.html)

[IHoleStandardsData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleStandardsData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0