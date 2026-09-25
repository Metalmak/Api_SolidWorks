<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressComponentContact.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SuppressUnsuppressComponentContact Method (ICWContactManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) : SuppressUnsuppressComponentContact Method (ICWContactManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   Name of component contact (see **Remarks**)

*BSuppress*
:   1 to suppress, 0 to unsuppress (see **Remarks**)

Obsolete. Superseded by [ICWContactManager::SuppressUnsuppressComponentContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressComponentContact2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SuppressUnsuppressComponentContact( _    ByVal SName As System.String, _    ByVal BSuppress As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactManager Dim SName As System.String Dim BSuppress As System.Integer Dim value As System.Integer   value = instance.SuppressUnsuppressComponentContact(SName, BSuppress) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SuppressUnsuppressComponentContact(     System.string SName,    System.int BSuppress ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SuppressUnsuppressComponentContact(  &   System.String^ SName, &   System.int BSuppress ) ``` | |

#### Parameters

*SName*
:   Name of component contact (see **Remarks**)

*BSuppress*
:   1 to suppress, 0 to unsuppress (see **Remarks**)

#### Return Value

Error code as defined in [swsContactSuppressUnsuppressError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSuppressUnsuppressError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactManager::SuppressUnsuppressComponentContact.

# ![](dotnetimages/collapse.gif)Example

[Add Component Contacts (VBA)](Add_Component_Contacts_Example_VB.htm)

[Add Component Contacts (VB.NET)](Add_Component_Contacts_Example_VBNET.htm)

[Add Component Contacts (C#)](Add_Component_Contacts_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, use:

* [ICWContactComponent::ContactName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactName.html) to get the name of the component contact.* [ICWContactComponent:State](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~State.html) to get the current suppression state of the component contact.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html)

[ICWContactComponent::SuppressUnSuppress Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~SuppressUnSuppress.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0