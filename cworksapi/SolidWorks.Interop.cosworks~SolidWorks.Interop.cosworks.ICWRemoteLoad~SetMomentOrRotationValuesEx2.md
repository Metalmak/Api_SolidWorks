<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValuesEx2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMomentOrRotationValuesEx2 Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetMomentOrRotationValuesEx2 Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   -1 or true to include moment or rotation in the remote load, 0 or false to not

*NXCode*
:   Remote load type in the x direction as defined in [swsRemoteLoadCheckCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadCheckCode_e.html)

*DXValue*
:   Moment or rotation in the x direction as specified by NXCode

*NYCode*
:   Remote load type in the y direction as defined in [swsRemoteLoadCheckCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadCheckCode_e.html)

*DYValue*
:   Moment or rotation in the y direction as specified by NYCode

*NZCode*
:   Remote load type in the z direction as defined in [swsRemoteLoadCheckCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadCheckCode_e.html)

*DZValue*
:   Moment or rotation in the z direction as specified by NZCode

Sets the components of moment or rotation for this remote load of a linear static, topology, or nonlinear static study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMomentOrRotationValuesEx2( _    ByVal BInclude As System.Boolean, _    ByVal NXCode As System.Integer, _    ByVal DXValue As System.Double, _    ByVal NYCode As System.Integer, _    ByVal DYValue As System.Double, _    ByVal NZCode As System.Integer, _    ByVal DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Boolean Dim NXCode As System.Integer Dim DXValue As System.Double Dim NYCode As System.Integer Dim DYValue As System.Double Dim NZCode As System.Integer Dim DZValue As System.Double   instance.SetMomentOrRotationValuesEx2(BInclude, NXCode, DXValue, NYCode, DYValue, NZCode, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMomentOrRotationValuesEx2(     System.bool BInclude,    System.int NXCode,    System.double DXValue,    System.int NYCode,    System.double DYValue,    System.int NZCode,    System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMomentOrRotationValuesEx2(  &   System.bool BInclude, &   System.int NXCode, &   System.double DXValue, &   System.int NYCode, &   System.double DYValue, &   System.int NZCode, &   System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   -1 or true to include moment or rotation in the remote load, 0 or false to not

*NXCode*
:   Remote load type in the x direction as defined in [swsRemoteLoadCheckCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadCheckCode_e.html)

*DXValue*
:   Moment or rotation in the x direction as specified by NXCode

*NYCode*
:   Remote load type in the y direction as defined in [swsRemoteLoadCheckCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadCheckCode_e.html)

*DYValue*
:   Moment or rotation in the y direction as specified by NYCode

*NZCode*
:   Remote load type in the z direction as defined in [swsRemoteLoadCheckCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsRemoteLoadCheckCode_e.html)

*DZValue*
:   Moment or rotation in the z direction as specified by NZCode

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWRemoteLoad::AllowDistributedCoupling2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~AllowDistributedCoupling2.html) returns -1 or true. If it returns 0 or false, then use [ICWRemoteLoad::SetMomentOrRotationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValues2.html) instead of this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30