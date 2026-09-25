<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpringConnector~SetSpringType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSpringType Method (ICWSpringConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSpringConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpringConnector.html) : SetSpringType Method (ICWSpringConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSpringType*
:   Spring type as defined in [swsSpringType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringType_e.html)

*NSpringSubType*
:   Spring sub type as defined in [swsSpringSubType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringSubType_e.html)

Sets the type of spring.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSpringType( _    ByVal NSpringType As System.Integer, _    ByVal NSpringSubType As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSpringConnector Dim NSpringType As System.Integer Dim NSpringSubType As System.Integer   instance.SetSpringType(NSpringType, NSpringSubType) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSpringType(     System.int NSpringType,    System.int NSpringSubType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSpringType(  &   System.int NSpringType, &   System.int NSpringSubType ) ``` | |

#### Parameters

*NSpringType*
:   Spring type as defined in [swsSpringType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringType_e.html)

*NSpringSubType*
:   Spring sub type as defined in [swsSpringSubType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringSubType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSpringConnector::SetSpringType.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSpringConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpringConnector.html)

[ICWSpringConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpringConnector_members.html)

[ICWSpringConnector::GetSpringType Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSpringConnector~GetSpringType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0