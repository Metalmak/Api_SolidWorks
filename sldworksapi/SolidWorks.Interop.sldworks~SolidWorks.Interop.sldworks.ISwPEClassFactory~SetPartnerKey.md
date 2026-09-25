<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory~SetPartnerKey.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPartnerKey Method (ISwPEClassFactory) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISwPEClassFactory Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory.html) : SetPartnerKey Method (ISwPEClassFactory) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StrPartnerEntitlement*
:   License key string (see **Remarks**)

*TokenObject*
:   [ISwPEToken](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEToken.html) (**for** **future use only - see Remarks**)

Sets the license key which SOLIDWORKS uses to verify SOLIDWORKS Partner entitlement.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPartnerKey( _    ByVal StrPartnerEntitlement As System.String, _    ByRef TokenObject As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwPEClassFactory Dim StrPartnerEntitlement As System.String Dim TokenObject As System.Object Dim value As System.Integer   value = instance.SetPartnerKey(StrPartnerEntitlement, TokenObject) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPartnerKey(     System.string StrPartnerEntitlement,    out System.object TokenObject ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPartnerKey(  &   System.String^ StrPartnerEntitlement, &   [Out] System.Object^ TokenObject ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StrPartnerEntitlement*
:   License key string (see **Remarks**)

*TokenObject*
:   [ISwPEToken](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEToken.html) (**for** **future use only - see Remarks**)

#### Return Value

Return code as defined by swPartnerEntitlementStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwPEClassFactory::SetPartnerKey.

# ![](dotnetimages/collapse.gif)Remarks

When this method is called, SOLIDWORKS compares the registry against these values in the license key specified in StrPartnerEntitlement:

* SOLIDWORKS Partner entitlement* SOLIDWORKS version* Add-in name* Add-in GUID* Expiration date

See SOLIDWORKS Partner Program.

TokenObject is for future use only.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwPEClassFactory Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory.html)

[ISwPEClassFactory Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISwPEClassFactory_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2021 FCS, Revision Number 29