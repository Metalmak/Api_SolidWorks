<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwPEManager~IdentifyToSW.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| IdentifyToSW Method (ISwPEManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwPEManager Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwPEManager.html) : IdentifyToSW Method (ISwPEManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ClassFactory*
:   Pointer to the ISwPEClassFactory dispatch object

Sends the specified callback object to the SOLIDWORKS Partner add-in, requesting a license key.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IdentifyToSW( _    ByVal ClassFactory As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwPEManager Dim ClassFactory As System.Object   instance.IdentifyToSW(ClassFactory) ``` | |

| C# |  |
| --- | --- |
| ``` void IdentifyToSW(     System.object ClassFactory ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IdentifyToSW(  &   System.Object^ ClassFactory ) ``` | |

#### Parameters

*ClassFactory*
:   Pointer to the ISwPEClassFactory dispatch object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwPEManager::IdentifyToSW.

# ![](dotnetimages/collapse.gif)Remarks

After receiving the ClassFactory dispatch object, the partner add-in calls ISwPEClassFactory::SetPartnerKey to send SOLIDWORKS a license key. SOLIDWORKS uses the partner key to verify entitlement of the SOLIDWORKS Partner.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwPEManager Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwPEManager.html)

[ISwPEManager Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwPEManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29