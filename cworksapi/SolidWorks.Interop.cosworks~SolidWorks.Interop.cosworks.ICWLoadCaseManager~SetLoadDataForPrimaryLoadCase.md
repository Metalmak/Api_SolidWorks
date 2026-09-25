<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~SetLoadDataForPrimaryLoadCase.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetLoadDataForPrimaryLoadCase Method (ICWLoadCaseManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadCaseManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html) : SetLoadDataForPrimaryLoadCase Method (ICWLoadCaseManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SLoadCaseName*
:   Name of primary load case

*SLoadName*
:   Name of load

*ArrayInputSuppressComps*
:   Array of booleans indicating which of the values in DataArrayInputVals to suppress; true to suppress, false to not

*DataArrayInputVals*
:   Array of values for SLoadName

Sets the load data for the specified primary load case and load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLoadDataForPrimaryLoadCase( _    ByVal SLoadCaseName As System.String, _    ByVal SLoadName As System.String, _    ByVal ArrayInputSuppressComps As System.Object, _    ByVal DataArrayInputVals As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadCaseManager Dim SLoadCaseName As System.String Dim SLoadName As System.String Dim ArrayInputSuppressComps As System.Object Dim DataArrayInputVals As System.Object Dim value As System.Integer   value = instance.SetLoadDataForPrimaryLoadCase(SLoadCaseName, SLoadName, ArrayInputSuppressComps, DataArrayInputVals) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetLoadDataForPrimaryLoadCase(     System.string SLoadCaseName,    System.string SLoadName,    System.object ArrayInputSuppressComps,    System.object DataArrayInputVals ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetLoadDataForPrimaryLoadCase(  &   System.String^ SLoadCaseName, &   System.String^ SLoadName, &   System.Object^ ArrayInputSuppressComps, &   System.Object^ DataArrayInputVals ) ``` | |

#### Parameters

*SLoadCaseName*
:   Name of primary load case

*SLoadName*
:   Name of load

*ArrayInputSuppressComps*
:   Array of booleans indicating which of the values in DataArrayInputVals to suppress; true to suppress, false to not

*DataArrayInputVals*
:   Array of values for SLoadName

#### Return Value

Error as defined in [swsLoadCaseManagerError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLoadCaseManagerError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadCaseManager::SetLoadDataForPrimaryLoadCase.

# ![](dotnetimages/collapse.gif)Example

See the [ICWLoadCaseManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWLoadCaseManager::GetAllPrimaryLoadCaseNames](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetAllPrimaryLoadCaseNames.html) to set SLoadCaseName.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadCaseManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html)

[ICWLoadCaseManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager_members.html)

[ICWLoadCaseManager::AddNewPrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~AddNewPrimaryLoadCase.html)

[ICWLoadCaseManager::DeletePrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~DeletePrimaryLoadCase.html)

[ICWLoadCaseManager::GetLoadDataForPrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetLoadDataForPrimaryLoadCase.html)

[ICWLoadCaseManager::GetSensorResultValueForPrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~GetSensorResultValueForPrimaryLoadCase.html)

[ICWLoadCaseManager::LoadResultsOfPrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~LoadResultsOfPrimaryLoadCase.html)

[ICWLoadCaseManager::RenamePrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~RenamePrimaryLoadCase.html)

[ICWLoadCaseManager::SuppressOrUnSuppressPrimaryLoadCase Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~SuppressOrUnSuppressPrimaryLoadCase.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0