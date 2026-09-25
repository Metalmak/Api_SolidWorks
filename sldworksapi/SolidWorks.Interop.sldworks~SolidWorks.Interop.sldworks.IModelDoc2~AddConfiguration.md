<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~AddConfiguration.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddConfiguration Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : AddConfiguration Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*

*Comment*

*AlternateName*

*SuppressByDefault*

*HideByDefault*

*MinFeatureManager*

*InheritProperties*

*Flags*

Obsolete. Superseded by [IModelDoc2::AddConfiguration3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~AddConfiguration3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub AddConfiguration( _    ByVal Name As System.String, _    ByVal Comment As System.String, _    ByVal AlternateName As System.String, _    ByVal SuppressByDefault As System.Boolean, _    ByVal HideByDefault As System.Boolean, _    ByVal MinFeatureManager As System.Boolean, _    ByVal InheritProperties As System.Boolean, _    ByVal Flags As System.UInteger _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Name As System.String Dim Comment As System.String Dim AlternateName As System.String Dim SuppressByDefault As System.Boolean Dim HideByDefault As System.Boolean Dim MinFeatureManager As System.Boolean Dim InheritProperties As System.Boolean Dim Flags As System.UInteger   instance.AddConfiguration(Name, Comment, AlternateName, SuppressByDefault, HideByDefault, MinFeatureManager, InheritProperties, Flags) ``` | |

| C# |  |
| --- | --- |
| ``` void AddConfiguration(     System.string Name,    System.string Comment,    System.string AlternateName,    System.bool SuppressByDefault,    System.bool HideByDefault,    System.bool MinFeatureManager,    System.bool InheritProperties,    System.uint Flags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddConfiguration(  &   System.String^ Name, &   System.String^ Comment, &   System.String^ AlternateName, &   System.bool SuppressByDefault, &   System.bool HideByDefault, &   System.bool MinFeatureManager, &   System.bool InheritProperties, &   System.uint Flags ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*Comment*

*AlternateName*

*SuppressByDefault*

*HideByDefault*

*MinFeatureManager*

*InheritProperties*

*Flags*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::AddConfiguration.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)