<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressContactPair.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SuppressUnsuppressContactPair Method (ICWContactManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) : SuppressUnsuppressContactPair Method (ICWContactManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   Name of contact set (see **Remarks**)

*BSuppress*
:   1 to suppress, 0 to unsuppress (see **Remarks**)

Obsolete. Superseded by [ICWContactManager::SuppressUnsuppressContactPair2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressContactPair2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SuppressUnsuppressContactPair( _    ByVal SName As System.String, _    ByVal BSuppress As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactManager Dim SName As System.String Dim BSuppress As System.Integer Dim value As System.Integer   value = instance.SuppressUnsuppressContactPair(SName, BSuppress) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SuppressUnsuppressContactPair(     System.string SName,    System.int BSuppress ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SuppressUnsuppressContactPair(  &   System.String^ SName, &   System.int BSuppress ) ``` | |

#### Parameters

*SName*
:   Name of contact set (see **Remarks**)

*BSuppress*
:   1 to suppress, 0 to unsuppress (see **Remarks**)

#### Return Value

Error code as defined in [swsContactSuppressUnsuppressError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSuppressUnsuppressError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactManager::SuppressUnsuppressContactPair.

# ![](dotnetimages/collapse.gif)Example

See the [ICWContactManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, use:

* [ICWContactSet::ContactName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~ContactName.html) to get the name of the contact set.* [ICWContactSet::State](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~State.html) to get the current suppression state of the contact set.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html)

[ICWContactSet::SuppressUnSuppress Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~SuppressUnSuppress.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0