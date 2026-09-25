<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~DeleteTrackResultsSensor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DeleteTrackResultsSensor Method (ICWLoadCaseManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadCaseManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html) : DeleteTrackResultsSensor Method (ICWLoadCaseManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SSensorName*
:   Name of data sensor to delete

Deletes the specified data sensor.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DeleteTrackResultsSensor( _    ByVal SSensorName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadCaseManager Dim SSensorName As System.String Dim value As System.Boolean   value = instance.DeleteTrackResultsSensor(SSensorName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DeleteTrackResultsSensor(     System.string SSensorName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DeleteTrackResultsSensor(  &   System.String^ SSensorName ) ``` | |

#### Parameters

*SSensorName*
:   Name of data sensor to delete

#### Return Value

True if deletion is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadCaseManager::DeleteTrackResultsSensor.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWLoadCaseManager::GetAllTrackResultsSensorNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetAllTrackResultsSensorNames.html) to set SSensorName.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadCaseManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html)

[ICWLoadCaseManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager_members.html)

[ICWLoadCaseManager::AddTrackResultsSensor Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~AddTrackResultsSensor.html)

[ICWLoadCaseManager::GetAllTrackResultsSensorNames Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetAllTrackResultsSensorNames.html)

[ICWLoadCaseManager::GetSensorResultValueForLoadCaseCombination Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetSensorResultValueForLoadCaseCombination.html)

[ICWLoadCaseManager::GetSensorResultValueForPrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetSensorResultValueForPrimaryLoadCase.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0