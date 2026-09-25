<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData~ISetTriadTranslationParameters.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetTriadTranslationParameters Method (IMoveFaceFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMoveFaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData.html) : ISetTriadTranslationParameters Method (IMoveFaceFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TranslationParameters*
:   * in-process, unmanaged C++: pointer to an array of three doubles for the X, Y, and Z translation parameters* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Sets the translation parameters for this Move Face feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ISetTriadTranslationParameters( _    ByRef TranslationParameters As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMoveFaceFeatureData Dim TranslationParameters As System.Double   instance.ISetTriadTranslationParameters(TranslationParameters) ``` | |

| C# |  |
| --- | --- |
| ``` void ISetTriadTranslationParameters(     ref System.double TranslationParameters ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ISetTriadTranslationParameters(  &   System.double% TranslationParameters ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*TranslationParameters*
:   * in-process, unmanaged C++: pointer to an array of three doubles for the X, Y, and Z translation parameters* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)See Also

####

[IMoveFaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData.html)

[IMoveFaceFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData_members.html)

[IMoveFaceFeatureData::IGetTriadTranslationParameters Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData~IGetTriadTranslationParameters.html)

[IMoveFaceFeatureData::TriadTranslationParameters Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveFaceFeatureData~TriadTranslationParameters.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0