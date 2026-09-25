<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplaceComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplaceComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ReplaceComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Path and new file name

*ConfigName*
:   Name of configuration

*ReplaceAllInstance*
:   True to replace all instances, false to not

*ReAttachMates*
:   True to reattach all of the mates if the component is found in the subassembly component, false to not

Obsolete. Superseded by [IAssemblyDoc::ReplaceComponents2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplaceComponents2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceComponents( _    ByVal FileName As System.String, _    ByVal ConfigName As System.String, _    ByVal ReplaceAllInstance As System.Boolean, _    ByVal ReAttachMates As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim FileName As System.String Dim ConfigName As System.String Dim ReplaceAllInstance As System.Boolean Dim ReAttachMates As System.Boolean Dim value As System.Boolean   value = instance.ReplaceComponents(FileName, ConfigName, ReplaceAllInstance, ReAttachMates) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplaceComponents(     System.string FileName,    System.string ConfigName,    System.bool ReplaceAllInstance,    System.bool ReAttachMates ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplaceComponents(  &   System.String^ FileName, &   System.String^ ConfigName, &   System.bool ReplaceAllInstance, &   System.bool ReAttachMates ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Path and new file name

*ConfigName*
:   Name of configuration

*ReplaceAllInstance*
:   True to replace all instances, false to not

*ReAttachMates*
:   True to reattach all of the mates if the component is found in the subassembly component, false to not

#### Return Value

True if the component is successfully replaced, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ReplaceComponents.

# ![](dotnetimages/collapse.gif)Remarks

You cannot replace a selected component with a component of the same name even if the components are in different folders.

The component must be a top-level component. It cannot be a component of a sub-assembly. If the application needs to replace a component of the sub-assembly, then it should open the sub-assembly and get the component from that assembly.

This method closes any component files when called in an assembly. If the components were modified, then those modifications are not automatically saved. You must save any modifications before closing the files.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponents.html)

[IAssemblyDoc::AddComponent5 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponent5.html)

[IAssemblyDoc::IAddComponents2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IAddComponents2.html)

[IModelDoc2::ReloadOrReplace Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ReloadOrReplace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0