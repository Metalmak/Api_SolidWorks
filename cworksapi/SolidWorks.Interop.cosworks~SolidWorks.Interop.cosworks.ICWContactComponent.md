<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWContactComponent Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWContactComponent Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to component contacts.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ICWContactComponent ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactComponent ``` | |

| C# |  |
| --- | --- |
| ``` public interface ICWContactComponent ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ICWContactComponent ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactComponent.

# ![](dotnetimages/collapse.gif)Example

[Add Component Contacts (VBA)](Add_Component_Contacts_Example_VB.htm)

[Add Component Contacts (VB.NET)](Add_Component_Contacts_Example_VBNET.htm)

[Add Component Contacts (C#)](Add_Component_Contacts_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Component contacts defined by [ICWContactManager::CreateContactComponent](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactManager~CreateContactComponent.html) override global contact conditions defined by [ICWContactManager::SetGlobalContact](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactManager~SetGlobalContact.html).

Contact sets defined by [ICWContactManager::CreateContactSet](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactManager~CreateContactSet.html) override both global and component contact definitions.

# ![](dotnetimages/collapse.gif)Accessors

[ICWContactManager::CreateContactComponent](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactManager~CreateContactComponent.html)

[ICWContactManager::GetContactComponentAt](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactManager~GetContactComponentAt.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactComponent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent_members.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactSet Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet.html)

[ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html)