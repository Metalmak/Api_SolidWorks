<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~EditConfiguration2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditConfiguration2 Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : EditConfiguration2 Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*

*NewName*

*Comment*

*AlternateName*

*SuppressByDefault*

*HideByDefault*

*MinFeatureManager*

*InheritProperties*

*Flags*

Obsolete. Superseded by [IModelDoc2::EditConfiguraiton2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditConfiguration2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EditConfiguration2( _    ByVal Name As System.String, _    ByVal NewName As System.String, _    ByVal Comment As System.String, _    ByVal AlternateName As System.String, _    ByVal SuppressByDefault As System.Boolean, _    ByVal HideByDefault As System.Boolean, _    ByVal MinFeatureManager As System.Boolean, _    ByVal InheritProperties As System.Boolean, _    ByVal Flags As System.UInteger _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Name As System.String Dim NewName As System.String Dim Comment As System.String Dim AlternateName As System.String Dim SuppressByDefault As System.Boolean Dim HideByDefault As System.Boolean Dim MinFeatureManager As System.Boolean Dim InheritProperties As System.Boolean Dim Flags As System.UInteger Dim value As System.Boolean   value = instance.EditConfiguration2(Name, NewName, Comment, AlternateName, SuppressByDefault, HideByDefault, MinFeatureManager, InheritProperties, Flags) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EditConfiguration2(     System.string Name,    System.string NewName,    System.string Comment,    System.string AlternateName,    System.bool SuppressByDefault,    System.bool HideByDefault,    System.bool MinFeatureManager,    System.bool InheritProperties,    System.uint Flags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool EditConfiguration2(  &   System.String^ Name, &   System.String^ NewName, &   System.String^ Comment, &   System.String^ AlternateName, &   System.bool SuppressByDefault, &   System.bool HideByDefault, &   System.bool MinFeatureManager, &   System.bool InheritProperties, &   System.uint Flags ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*NewName*

*Comment*

*AlternateName*

*SuppressByDefault*

*HideByDefault*

*MinFeatureManager*

*InheritProperties*

*Flags*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::EditConfiguration2.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)