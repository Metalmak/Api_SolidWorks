<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~MirrorComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MirrorComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : MirrorComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Plane*
:   Plane or planar face about which to mirror the components

*ComponentsToInstance*
:   Array of instances of the component to mirror

*ComponentsToMirror*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to mirror

*MirroredComponentFilenames*
:   Array of filenames for the newly created mirrored assemblies or parts

*RecreateMates*
:   True to preserve any mates between the selected components if more than one component is to be mirrored, false to not

*ComponentModifier*
:   Prefix or suffix for the newly mirrored components if MirroredComponentFilenames is not specified, as defined by swMirrorComponentNameModifier\_e

*ComponentNameModifier*
:   String to add to the prefix or suffix of the name of the newly mirrored component if MirroredComponentFilenames is not specified

*MirroredFileLocation*
:   Name of the folder where to store the file of the newly created mirrored components

*CopyCustomProperties*
:   True to copy the custom properties from the selected components to the mirrored components, false to not

Obsolete. Superseded by [IAssemblyDoc::MirrorComponents2.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~MirrorComponents2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MirrorComponents( _    ByVal Plane As System.Object, _    ByVal ComponentsToInstance As System.Object, _    ByVal ComponentsToMirror As System.Object, _    ByVal MirroredComponentFilenames As System.Object, _    ByVal RecreateMates As System.Boolean, _    ByVal ComponentModifier As System.Integer, _    ByVal ComponentNameModifier As System.String, _    ByVal MirroredFileLocation As System.String, _    ByVal CopyCustomProperties As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Plane As System.Object Dim ComponentsToInstance As System.Object Dim ComponentsToMirror As System.Object Dim MirroredComponentFilenames As System.Object Dim RecreateMates As System.Boolean Dim ComponentModifier As System.Integer Dim ComponentNameModifier As System.String Dim MirroredFileLocation As System.String Dim CopyCustomProperties As System.Boolean Dim value As System.Object   value = instance.MirrorComponents(Plane, ComponentsToInstance, ComponentsToMirror, MirroredComponentFilenames, RecreateMates, ComponentModifier, ComponentNameModifier, MirroredFileLocation, CopyCustomProperties) ``` | |

| C# |  |
| --- | --- |
| ``` System.object MirrorComponents(     System.object Plane,    System.object ComponentsToInstance,    System.object ComponentsToMirror,    System.object MirroredComponentFilenames,    System.bool RecreateMates,    System.int ComponentModifier,    System.string ComponentNameModifier,    System.string MirroredFileLocation,    System.bool CopyCustomProperties ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ MirrorComponents(  &   System.Object^ Plane, &   System.Object^ ComponentsToInstance, &   System.Object^ ComponentsToMirror, &   System.Object^ MirroredComponentFilenames, &   System.bool RecreateMates, &   System.int ComponentModifier, &   System.String^ ComponentNameModifier, &   System.String^ MirroredFileLocation, &   System.bool CopyCustomProperties ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Plane*
:   Plane or planar face about which to mirror the components

*ComponentsToInstance*
:   Array of instances of the component to mirror

*ComponentsToMirror*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to mirror

*MirroredComponentFilenames*
:   Array of filenames for the newly created mirrored assemblies or parts

*RecreateMates*
:   True to preserve any mates between the selected components if more than one component is to be mirrored, false to not

*ComponentModifier*
:   Prefix or suffix for the newly mirrored components if MirroredComponentFilenames is not specified, as defined by swMirrorComponentNameModifier\_e

*ComponentNameModifier*
:   String to add to the prefix or suffix of the name of the newly mirrored component if MirroredComponentFilenames is not specified

*MirroredFileLocation*
:   Name of the folder where to store the file of the newly created mirrored components

*CopyCustomProperties*
:   True to copy the custom properties from the selected components to the mirrored components, false to not

#### Return Value

Array of the newly created [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::MirrorComponents.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0