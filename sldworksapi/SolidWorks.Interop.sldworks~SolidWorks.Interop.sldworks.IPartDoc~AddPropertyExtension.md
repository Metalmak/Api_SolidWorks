<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~AddPropertyExtension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddPropertyExtension Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : AddPropertyExtension Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PropertyExtension*
:   Value of the property extension to add to this part (see **Remarks**)

Adds a property extension to this part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddPropertyExtension( _    ByVal PropertyExtension As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim PropertyExtension As System.Object Dim value As System.Integer   value = instance.AddPropertyExtension(PropertyExtension) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddPropertyExtension(     System.object PropertyExtension ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddPropertyExtension(  &   System.Object^ PropertyExtension ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PropertyExtension*
:   Value of the property extension to add to this part (see **Remarks**)

#### Return Value

Size of the array to which the property extension value is added

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::AddPropertyExtension.

# ![](dotnetimages/collapse.gif)Example

[Add and Get Property Extensions (C#)](Add_and_Get_Property_Extension_Example_CSharp.htm)

[Add and Get Property Extensions (VB.NET)](Add_and_Get_Property_Extension_Example_VBNET.htm)

[Add and Get Property Extensions (VBA)](Add_and_Get_Property_Extension_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To use this method:

1. Declare the variable.- Assign the variable a value: float, integer, or string.- Call this method to add the value to the part.

The 1-based array is a first-in-last-out structured list, whose size is used by [IPartDoc::GetPropertyExtension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~GetPropertyExtension.html) to access the property extension. See the examples in **Example**.

**NOTE**: SOLIDWORKS recommends that you use the [IAttribute](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttribute.html), [IAttributeDef](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef.html), and [IParameter](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IParameter.html) interfaces instead of this method. These interfaces provide more flexibility.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::ResetPropertyExtension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ResetPropertyExtension.html)