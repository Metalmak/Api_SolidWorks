<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~GetPrincipalMomentOfInertia.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPrincipalMomentOfInertia Method (ICWMassPropertiesManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMassPropertiesManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager.html) : GetPrincipalMomentOfInertia Method (ICWMassPropertiesManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the moments of inertia with respect to the principal axes and the center of mass.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPrincipalMomentOfInertia() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMassPropertiesManager Dim value As System.Object   value = instance.GetPrincipalMomentOfInertia() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPrincipalMomentOfInertia() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPrincipalMomentOfInertia(); ``` | |

#### Return Value

Array of three principal moments of inertia (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMassPropertiesManager::GetPrincipalMomentOfInertia.

# ![](dotnetimages/collapse.gif)Example

See the [ICWMassPropertiesManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The moment of inertia is calculated with respect to the output coordinate system. Before calling this method, call [ICWMassPropertiesManager::SetCoordinateSystemName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~SetCoordinateSystemName.html) or [ICWMassPropertiesManager::SetCoordinateSystemToDefault](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~SetCoordinateSystemToDefault.html).

The moments of inertia are in units of kilograms \* meters squared.

This method returns three doubles as follows:

     [ *Px*, *Py*, *Pz* ]

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMassPropertiesManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager.html)

[ICWMassPropertiesManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager_members.html)

[ICWMassPropertiesManager::GetMomentOfInertia Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~GetMomentOfInertia.html)

[ICWMassPropertiesManager::GetMomentOfInertiaAtOutputCoordinateSystem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~GetMomentOfInertiaAtOutputCoordinateSystem.html)

[ICWMassPropertiesManager::GetPrincipalAxesOfInertia Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMassPropertiesManager~GetPrincipalAxesOfInertia.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0