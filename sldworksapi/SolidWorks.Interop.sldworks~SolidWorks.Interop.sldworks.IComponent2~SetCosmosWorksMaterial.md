<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~SetCosmosWorksMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetCosmosWorksMaterial Method (IComponent2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) : SetCosmosWorksMaterial Method (IComponent2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ConfigName*
:   Name of the configuration

*Type*
:   Type of material to assign as defined by swCosmosWorksMat

Assigns the material to use during analysis to this component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCosmosWorksMaterial( _    ByVal ConfigName As System.String, _    ByVal Type As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IComponent2 Dim ConfigName As System.String Dim Type As System.Integer Dim value As System.Boolean   value = instance.SetCosmosWorksMaterial(ConfigName, Type) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetCosmosWorksMaterial(     System.string ConfigName,    System.int Type ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetCosmosWorksMaterial(  &   System.String^ ConfigName, &   System.int Type ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ConfigName*
:   Name of the configuration

*Type*
:   Type of material to assign as defined by swCosmosWorksMat

#### Return Value

True if the material is assigned, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Component2::SetCosmosWorksMaterial.

# ![](dotnetimages/collapse.gif)See Also

####

[IComponent2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

[IComponent2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2_members.html)

[IPartDoc::SetCosmosWorksMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~SetCosmosWorksMaterial.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0