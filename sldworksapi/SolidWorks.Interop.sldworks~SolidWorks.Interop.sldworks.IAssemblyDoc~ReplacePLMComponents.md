<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplacePLMComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplacePLMComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ReplacePLMComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PLMID*
:   Unique ID of a replacement component in the collaboration space

*ConfigName*
:   Name of a configuration (Physical Product) in the replacement component; an empty string indicates the default configuration of the replacement component

*ReplaceAllInstance*
:   True to replace all instances of the selected components with the replacement component, false to not

*UseConfigChoice*
:   Configuration to use as defined in swReplaceComponentsConfiguration\_e

*ReAttachMates*
:   True to reattach any existing mates to the replacement component, false to not

Replaces a selected SOLIDWORKS Connected component in this assembly with the specified component from a 3DEXPERIENCE collaborative space.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplacePLMComponents( _    ByVal PLMID As System.String, _    ByVal ConfigName As System.String, _    ByVal ReplaceAllInstance As System.Boolean, _    ByVal UseConfigChoice As System.Integer, _    ByVal ReAttachMates As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim PLMID As System.String Dim ConfigName As System.String Dim ReplaceAllInstance As System.Boolean Dim UseConfigChoice As System.Integer Dim ReAttachMates As System.Boolean Dim value As System.Boolean   value = instance.ReplacePLMComponents(PLMID, ConfigName, ReplaceAllInstance, UseConfigChoice, ReAttachMates) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplacePLMComponents(     System.string PLMID,    System.string ConfigName,    System.bool ReplaceAllInstance,    System.int UseConfigChoice,    System.bool ReAttachMates ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplacePLMComponents(  &   System.String^ PLMID, &   System.String^ ConfigName, &   System.bool ReplaceAllInstance, &   System.int UseConfigChoice, &   System.bool ReAttachMates ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PLMID*
:   Unique ID of a replacement component in the collaboration space

*ConfigName*
:   Name of a configuration (Physical Product) in the replacement component; an empty string indicates the default configuration of the replacement component

*ReplaceAllInstance*
:   True to replace all instances of the selected components with the replacement component, false to not

*UseConfigChoice*
:   Configuration to use as defined in swReplaceComponentsConfiguration\_e

*ReAttachMates*
:   True to reattach any existing mates to the replacement component, false to not

#### Return Value

True if the selected component is replaced, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ReplacePLMComponents.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, save any components that have been modified in this assembly. This method closes any open component files without saving modifications.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddPLMComponent Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddPLMComponent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30