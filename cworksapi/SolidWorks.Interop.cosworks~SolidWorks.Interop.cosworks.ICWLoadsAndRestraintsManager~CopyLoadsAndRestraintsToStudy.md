<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~CopyLoadsAndRestraintsToStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CopyLoadsAndRestraintsToStudy Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : CopyLoadsAndRestraintsToStudy Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SStudyName*
:   Name of study to which to copy loads and restraints

*LRNames*
:   Array of names of loads and restraints to copy (see **Remarks**)

Copies the specified loads and restraints to the specified study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CopyLoadsAndRestraintsToStudy( _    ByVal SStudyName As System.String, _    ByVal LRNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim SStudyName As System.String Dim LRNames As System.Object Dim value As System.Integer   value = instance.CopyLoadsAndRestraintsToStudy(SStudyName, LRNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CopyLoadsAndRestraintsToStudy(     System.string SStudyName,    System.object LRNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CopyLoadsAndRestraintsToStudy(  &   System.String^ SStudyName, &   System.Object^ LRNames ) ``` | |

#### Parameters

*SStudyName*
:   Name of study to which to copy loads and restraints

*LRNames*
:   Array of names of loads and restraints to copy (see **Remarks**)

#### Return Value

Error code as defined in [swsCopyItemsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCopyItemsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::CopyLoadsAndRestraintsToStudy.

# ![](dotnetimages/collapse.gif)Example

[Copy Items to Another Study (VBA)](Copy_Items_to_Another_Study_Example_VB.htm)

[Copy Items to Another Study (VB.NET)](Copy_Items_to_Another_Study_Example_VBNET.htm)

[Copy Items to Another Study (C#)](Copy_Items_to_Another_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To populate the array of LRNames, either:

* inspect the Simulation study tree.

- or -

* call [ICWLoadsAndRestraintsManager::GetLoadsAndRestraints](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~GetLoadsAndRestraints.html) to get each [ICWLoadsAndRestraints](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints.html) and then call [ICWLoadsAndRestraints::Name](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints~Name.html) to get the name of each load or restraint.

If a load or restraint name already exists, **Copy[1]** is prepended to the name of the copied load or restraint.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

[ICWLoadsAndRestraintsManager::DeleteLoadsAndRestraints Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~DeleteLoadsAndRestraints.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0