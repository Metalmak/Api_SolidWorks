<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~RunLoadCases.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| RunLoadCases Method (ICWLoadCaseManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadCaseManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html) : RunLoadCases Method (ICWLoadCaseManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BPrimaryLoadCases*
:   True to use primary load cases, false to not

*BLoadCaseCombinations*
:   True to use load case combinations, false to not

Runs the analysis using primary load cases, primary load case combinations, or both.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunLoadCases( _    ByVal BPrimaryLoadCases As System.Boolean, _    ByVal BLoadCaseCombinations As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadCaseManager Dim BPrimaryLoadCases As System.Boolean Dim BLoadCaseCombinations As System.Boolean Dim value As System.Integer   value = instance.RunLoadCases(BPrimaryLoadCases, BLoadCaseCombinations) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunLoadCases(     System.bool BPrimaryLoadCases,    System.bool BLoadCaseCombinations ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunLoadCases(  &   System.bool BPrimaryLoadCases, &   System.bool BLoadCaseCombinations ) ``` | |

#### Parameters

*BPrimaryLoadCases*
:   True to use primary load cases, false to not

*BLoadCaseCombinations*
:   True to use load case combinations, false to not

#### Return Value

Error as defined in [swsLoadCaseManagerError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLoadCaseManagerError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadCaseManager::RunLoadCases.

# ![](dotnetimages/collapse.gif)Example

See the [ICWLoadCaseManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadCaseManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager.html)

[ICWLoadCaseManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager_members.html)

[ICWLoadCaseManager::CloseLoadCaseManager Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~CloseLoadCaseManager.html)

[ICWLoadCaseManager::OpenLoadCaseManager Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~OpenLoadCaseManager.html)

[ICWLoadCaseManager::DeleteAllDataAndClose Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadCaseManager~DeleteAllDataAndClose.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0