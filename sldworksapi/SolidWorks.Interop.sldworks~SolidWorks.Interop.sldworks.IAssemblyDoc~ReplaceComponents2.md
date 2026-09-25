<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplaceComponents2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplaceComponents2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ReplaceComponents2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Path and file name of the replacement component

*ConfigName*
:   Name of a configuration in the replacement component; an empty string indicates the default configuration of the replacement component

*ReplaceAllInstance*
:   True to replace all instances of the selected components with the replacement component, false to not

*UseConfigChoice*
:   Configuration to use as defined in swReplaceComponentsConfiguration\_e

*ReAttachMates*
:   True to reattach existing mates to the replacement component, false to not

Replaces one or more selected components with another model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceComponents2( _    ByVal FileName As System.String, _    ByVal ConfigName As System.String, _    ByVal ReplaceAllInstance As System.Boolean, _    ByVal UseConfigChoice As System.Integer, _    ByVal ReAttachMates As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim FileName As System.String Dim ConfigName As System.String Dim ReplaceAllInstance As System.Boolean Dim UseConfigChoice As System.Integer Dim ReAttachMates As System.Boolean Dim value As System.Boolean   value = instance.ReplaceComponents2(FileName, ConfigName, ReplaceAllInstance, UseConfigChoice, ReAttachMates) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplaceComponents2(     System.string FileName,    System.string ConfigName,    System.bool ReplaceAllInstance,    System.int UseConfigChoice,    System.bool ReAttachMates ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplaceComponents2(  &   System.String^ FileName, &   System.String^ ConfigName, &   System.bool ReplaceAllInstance, &   System.int UseConfigChoice, &   System.bool ReAttachMates ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Path and file name of the replacement component

*ConfigName*
:   Name of a configuration in the replacement component; an empty string indicates the default configuration of the replacement component

*ReplaceAllInstance*
:   True to replace all instances of the selected components with the replacement component, false to not

*UseConfigChoice*
:   Configuration to use as defined in swReplaceComponentsConfiguration\_e

*ReAttachMates*
:   True to reattach existing mates to the replacement component, false to not

#### Return Value

True if the selected components are replaced, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ReplaceComponents2.

# ![](dotnetimages/collapse.gif)Example

[Replace Component (C#)](Replace_Component_Example_CSharp.htm)

[Replace Component (VB.NET)](Replace_Component_Example_VBNET.htm)

[Replace Component (VBA)](Replace_Component_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You cannot replace a selected component with a component of the same name even if the components reside in different folders.

The component must be a top-level component. It cannot be a component of a sub-assembly. If your application needs to replace a component of a sub-assembly, then your application must open the sub-assembly and get the component from that assembly.

This method closes any component files when called in an assembly. If components were modified, then those modifications are not automatically saved. You must save any modifications before closing the files.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IModelDoc2::ReloadOrReplace Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ReloadOrReplace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0