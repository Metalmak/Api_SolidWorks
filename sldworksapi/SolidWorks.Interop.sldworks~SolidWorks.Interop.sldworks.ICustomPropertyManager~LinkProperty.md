<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~LinkProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| LinkProperty Method (ICustomPropertyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html) : LinkProperty Method (ICustomPropertyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FieldName*
:   Name of the custom property to link or unlink

*FieldLink*
:   True to link the custom property, false to unlink it

Sets whether to link or unlink the specified custom property to or from its parent part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function LinkProperty( _    ByVal FieldName As System.String, _    ByVal FieldLink As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICustomPropertyManager Dim FieldName As System.String Dim FieldLink As System.Boolean Dim value As System.Integer   value = instance.LinkProperty(FieldName, FieldLink) ``` | |

| C# |  |
| --- | --- |
| ``` System.int LinkProperty(     System.string FieldName,    System.bool FieldLink ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int LinkProperty(  &   System.String^ FieldName, &   System.bool FieldLink ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FieldName*
:   Name of the custom property to link or unlink

*FieldLink*
:   True to link the custom property, false to unlink it

#### Return Value

Result code as defined in swCustomLinkSetResult\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CustomPropertyManager::LinkProperty.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid for cut-list, feature, model, and configuration custom properties.

# ![](dotnetimages/collapse.gif)See Also

####

[ICustomPropertyManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager.html)

[ICustomPropertyManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager_members.html)

[ICustomPropertyManager::LinkAll Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICustomPropertyManager~LinkAll.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0