<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddDistributedMass.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddDistributedMass Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddDistributedMass Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispArray*
:   Array of faces or shell edges on which to distribute the mass

*NUnits*
:   Units as defined in [swsUnitSystem\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnitSystem_e.html)

*DMass*
:   Mass to distribute

*ErrorCode*
:   Error code as defined in [swsDistributedMassError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDistributedMassError_e.html)

Creates a distributed mass.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDistributedMass( _    ByVal DispArray As System.Object, _    ByVal NUnits As System.Integer, _    ByVal DMass As System.Double, _    ByRef ErrorCode As System.Integer _ ) As CWDistributedMass ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim DispArray As System.Object Dim NUnits As System.Integer Dim DMass As System.Double Dim ErrorCode As System.Integer Dim value As CWDistributedMass   value = instance.AddDistributedMass(DispArray, NUnits, DMass, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWDistributedMass AddDistributedMass(     System.object DispArray,    System.int NUnits,    System.double DMass,    ref System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWDistributedMass^ AddDistributedMass(  &   System.Object^ DispArray, &   System.int NUnits, &   System.double DMass, &   System.int% ErrorCode ) ``` | |

#### Parameters

*DispArray*
:   Array of faces or shell edges on which to distribute the mass

*NUnits*
:   Units as defined in [swsUnitSystem\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnitSystem_e.html)

*DMass*
:   Mass to distribute

*ErrorCode*
:   Error code as defined in [swsDistributedMassError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDistributedMassError_e.html)

#### Return Value

[ICWDistributedMass](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDistributedMass.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddDistributedMass.

# ![](dotnetimages/collapse.gif)Example

[Create Linear Dynamic Study (C#)](Create_Dynamic_Harmonic_Study_Example_CSharp.htm)

[Create Linear Dynamic Study (VB.NET)](Create_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Linear Dynamic Study (VBA)](Create_Dynamic_Harmonic_Study_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0