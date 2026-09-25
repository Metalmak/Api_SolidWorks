<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateContactComponent Method (ICWContactManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) : CreateContactComponent Method (ICWContactManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NContactType*
:   Type of component contact for:

    * [static](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStaticStudyOptions.html), [nonlinear](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWNonLinearStudyOptions.html), [buckling](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBucklingStudyOptions.html) and [thermal](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWThermalStudyOptions.html) studies as defined in [swsContactType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsContactType_e.html)* [frequency](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWFrequencyStudyOptions.html) studies as defined in [swsContactType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsContactType_e.html), excluding swsContactTypeStaticNoPenetration

*NOption*
:   Mesh compatibility as defined in [swsMeshCompatibility\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshCompatibility_e.html)

*DispEntity*
:   Component entity

*ErrorCode*
:   Error code as defined in [swsContactComponentEndEditError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactComponentEndEditError_e.html)

Creates the specified component contact.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateContactComponent( _    ByVal NContactType As System.Integer, _    ByVal NOption As System.Integer, _    ByVal DispEntity As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWContactComponent ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactManager Dim NContactType As System.Integer Dim NOption As System.Integer Dim DispEntity As System.Object Dim ErrorCode As System.Integer Dim value As CWContactComponent   value = instance.CreateContactComponent(NContactType, NOption, DispEntity, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWContactComponent CreateContactComponent(     System.int NContactType,    System.int NOption,    System.object DispEntity,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWContactComponent^ CreateContactComponent(  &   System.int NContactType, &   System.int NOption, &   System.Object^ DispEntity, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NContactType*
:   Type of component contact for:

    * [static](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStaticStudyOptions.html), [nonlinear](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWNonLinearStudyOptions.html), [buckling](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBucklingStudyOptions.html) and [thermal](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWThermalStudyOptions.html) studies as defined in [swsContactType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsContactType_e.html)* [frequency](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWFrequencyStudyOptions.html) studies as defined in [swsContactType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsContactType_e.html), excluding swsContactTypeStaticNoPenetration

*NOption*
:   Mesh compatibility as defined in [swsMeshCompatibility\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsMeshCompatibility_e.html)

*DispEntity*
:   Component entity

*ErrorCode*
:   Error code as defined in [swsContactComponentEndEditError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactComponentEndEditError_e.html)

#### Return Value

[Component contact](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactComponent.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactManager::CreateContactComponent.

# ![](dotnetimages/collapse.gif)Example

[Add Component Contacts (VBA)](Add_Component_Contacts_Example_VB.htm)

[Add Component Contacts (VB.NET)](Add_Component_Contacts_Example_VBNET.htm)

[Add Component Contacts (C#)](Add_Component_Contacts_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

See the SOLIDWORKS Simulation Help for guidelines about studies with contact conditions.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html)

[ICWContactManager::DeleteContactComponent Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~DeleteContactComponent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0