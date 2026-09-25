<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CopyWithMates.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CopyWithMates Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : CopyWithMates Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentsToCopy*
:   Array of [components](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) to copy

*Repeat*
:   Array of boolean values; each value indicates whether to use the existing mate reference for the corresponding component to copy: if true, copies the existing mate reference; if false, uses the corresponding entry in the NewEntityToMateTo array for the new mate reference

*NewEnityToMateTo*
:   Array of new mate references that map to the Repeat arrays; if an entry in the Repeat array is false, then the corresponding entry in this array is the new entity with which to mate the component to copy

*Values*
:   Array of distance or angle values for the mate references; specify distance in meters and angle in radians; valid for for distance and angle mates only

*FlipAlignment*
:   Array of booleans that map to the NewEntityToMateTo array; each value indicates the corresponding mate's alignment; true to flip alignment, false otherwise; valid for distance and angle mates only

Obsolete. Superseded by [IAssemblyDoc::CopyWithMates2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CopyWithMates2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CopyWithMates( _    ByVal ComponentsToCopy As System.Object, _    ByVal Repeat As System.Object, _    ByVal NewEnityToMateTo As System.Object, _    ByVal Values As System.Object, _    ByVal FlipAlignment As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim ComponentsToCopy As System.Object Dim Repeat As System.Object Dim NewEnityToMateTo As System.Object Dim Values As System.Object Dim FlipAlignment As System.Object Dim value As System.Boolean   value = instance.CopyWithMates(ComponentsToCopy, Repeat, NewEnityToMateTo, Values, FlipAlignment) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CopyWithMates(     System.object ComponentsToCopy,    System.object Repeat,    System.object NewEnityToMateTo,    System.object Values,    System.object FlipAlignment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CopyWithMates(  &   System.Object^ ComponentsToCopy, &   System.Object^ Repeat, &   System.Object^ NewEnityToMateTo, &   System.Object^ Values, &   System.Object^ FlipAlignment ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ComponentsToCopy*
:   Array of [components](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) to copy

*Repeat*
:   Array of boolean values; each value indicates whether to use the existing mate reference for the corresponding component to copy: if true, copies the existing mate reference; if false, uses the corresponding entry in the NewEntityToMateTo array for the new mate reference

*NewEnityToMateTo*
:   Array of new mate references that map to the Repeat arrays; if an entry in the Repeat array is false, then the corresponding entry in this array is the new entity with which to mate the component to copy

*Values*
:   Array of distance or angle values for the mate references; specify distance in meters and angle in radians; valid for for distance and angle mates only

*FlipAlignment*
:   Array of booleans that map to the NewEntityToMateTo array; each value indicates the corresponding mate's alignment; true to flip alignment, false otherwise; valid for distance and angle mates only

#### Return Value

True if calling this method succeeded; false if it failed

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::CopyWithMates.

# ![](dotnetimages/collapse.gif)Example

[Copy Components With Mates to Assembly (VBA)](Copy_Components_With_Mates_To_Assembly_Example_VB.htm)

[Copy Components With Mates to Assembly (VB.NET)](Copy_Components_With_Mates_To_Assembly_Example_VBNET.htm)

[Copy Components With Mates to Assembly (C#)](Copy_Components_With_Mates_To_Assembly_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0