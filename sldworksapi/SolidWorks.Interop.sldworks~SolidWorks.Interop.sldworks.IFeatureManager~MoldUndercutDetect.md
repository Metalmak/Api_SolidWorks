<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~MoldUndercutDetect.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoldUndercutDetect Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : MoldUndercutDetect Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ColUndercut*

*ColBase*

*BCoordInput*

*Dx*

*Dy*

*Dz*

Obsolete. Superseded by [IFeatureManager::MoldUndercutDetect2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~MoldUndercutDetect2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub MoldUndercutDetect( _    ByVal ColUndercut As System.Integer, _    ByVal ColBase As System.Integer, _    ByVal BCoordInput As System.Boolean, _    ByVal Dx As System.Double, _    ByVal Dy As System.Double, _    ByVal Dz As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim ColUndercut As System.Integer Dim ColBase As System.Integer Dim BCoordInput As System.Boolean Dim Dx As System.Double Dim Dy As System.Double Dim Dz As System.Double   instance.MoldUndercutDetect(ColUndercut, ColBase, BCoordInput, Dx, Dy, Dz) ``` | |

| C# |  |
| --- | --- |
| ``` void MoldUndercutDetect(     System.int ColUndercut,    System.int ColBase,    System.bool BCoordInput,    System.double Dx,    System.double Dy,    System.double Dz ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void MoldUndercutDetect(  &   System.int ColUndercut, &   System.int ColBase, &   System.bool BCoordInput, &   System.double Dx, &   System.double Dy, &   System.double Dz ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ColUndercut*

*ColBase*

*BCoordInput*

*Dx*

*Dy*

*Dz*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::MoldUndercutDetect.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)