<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISwPEClassFactory Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISwPEClassFactory Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the callback object used by ISwPEManager to send a license key back to SOLIDWORKS for SOLIDWORKS Partner entitlement verification.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwPEClassFactory ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwPEClassFactory ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwPEClassFactory ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwPEClassFactory ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwPEClassFactory.

# ![](dotnetimages/collapse.gif)Remarks

This interface provides a callback mechanism in which:

1. SOLIDWORKS requests the partner's key through the add-in by calling ISwPEManager::IdentifyToSW,- The partner add-in sends a license key back to SOLIDWORKS in [ISwPEClassFactory::SetPartnerKey](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory~SetPartnerKey.html), and- SOLIDWORKS uses the license key to verify the entitlement of the SOLIDWORKS Partner and returns [ISwPEToken](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEToken.html).

 See SOLIDWORKS Partner Program.

# ![](dotnetimages/collapse.gif)Accessors

ISwPEManager::IdentifyToSW

# ![](dotnetimages/collapse.gif)See Also

####

[ISwPEClassFactory Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)