<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CopyContactsToStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CopyContactsToStudy Method (ICWContactManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) : CopyContactsToStudy Method (ICWContactManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SStudyName*
:   Name of study to which to copy contact sets

*VarContactNames*
:   Array of contact names (see **Remarks**)

Copies the specified contact sets to the specified study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CopyContactsToStudy( _    ByVal SStudyName As System.String, _    ByVal VarContactNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactManager Dim SStudyName As System.String Dim VarContactNames As System.Object Dim value As System.Integer   value = instance.CopyContactsToStudy(SStudyName, VarContactNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int CopyContactsToStudy(     System.string SStudyName,    System.object VarContactNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CopyContactsToStudy(  &   System.String^ SStudyName, &   System.Object^ VarContactNames ) ``` | |

#### Parameters

*SStudyName*
:   Name of study to which to copy contact sets

*VarContactNames*
:   Array of contact names (see **Remarks**)

#### Return Value

Error code as defined in [swsCopyItemsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCopyItemsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactManager::CopyContactsToStudy.

# ![](dotnetimages/collapse.gif)Example

[Copy Items to Another Study (VBA)](Copy_Items_to_Another_Study_Example_VB.htm)

[Copy Items to Another Study (VB.NET)](Copy_Items_to_Another_Study_Example_VBNET.htm)

[Copy Items to Another Study (C#)](Copy_Items_to_Another_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To populate the array of VarContactNames, either:

* inspect **Connections > Contact Sets** in the Simulation study tree.

- or -

* call [ICWContactManager::GetContactSetAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~GetContactSetAt.html) to get each [ICWContactSet](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet.html) and then call [ICWContactSet::ContactName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~ContactName.html) to get the name of each contact set.

If a contact set name already exists, **Copy[1]** is prepended to the name of the copied contact set.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0