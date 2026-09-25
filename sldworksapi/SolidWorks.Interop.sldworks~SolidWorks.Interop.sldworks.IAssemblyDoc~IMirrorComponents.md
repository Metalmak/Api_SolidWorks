<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IMirrorComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMirrorComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : IMirrorComponents Method (IAssemblyDoc) |

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

*InstanceCount*
:   Number of instances of the components to mirror

*ComponentsToInstance*
:   Array of instances of the [component](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to mirror

*MirrorCount*
:   Number of components to mirror

*ComponentsToMirror*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to mirror

*NameCount*
:   Number of filenames for the newly created mirrored assemblies or parts

*MirroredComponentFilenames*
:   Array of filenames for the newly created mirrored assemblies or parts

*RecreateMates*
:   True to preserve any mates between the selected components if more than one component is to be mirrored, false to not

*ComponentModifier*
:   Prefix or suffix for the newly mirrored components if MirroredComponentFilenames is not specified, as defined by swMirrorComponentNameModifier\_e

*ComponentNameModifier*
:   String to add to the prefix or suffix of the name of the newly mirrored components if MirroredComponentFilenames is not specified

*MirroredFileLocation*
:   Name of the folder where to store the file of the newly created mirrored components

*CopyCustomProperties*
:   True to copy the custom properties from the selected components to the mirrored components, false to not

Obsolete. Superseded by [IAssemblyDoc::MirrorComponents2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~MirrorComponents2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IMirrorComponents( _    ByVal Plane As System.Object, _    ByVal InstanceCount As System.Integer, _    ByRef ComponentsToInstance As Component2, _    ByVal MirrorCount As System.Integer, _    ByRef ComponentsToMirror As Component2, _    ByVal NameCount As System.Integer, _    ByRef MirroredComponentFilenames As System.String, _    ByVal RecreateMates As System.Boolean, _    ByVal ComponentModifier As System.Integer, _    ByVal ComponentNameModifier As System.String, _    ByVal MirroredFileLocation As System.String, _    ByVal CopyCustomProperties As System.Boolean _ ) As Component2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim Plane As System.Object Dim InstanceCount As System.Integer Dim ComponentsToInstance As Component2 Dim MirrorCount As System.Integer Dim ComponentsToMirror As Component2 Dim NameCount As System.Integer Dim MirroredComponentFilenames As System.String Dim RecreateMates As System.Boolean Dim ComponentModifier As System.Integer Dim ComponentNameModifier As System.String Dim MirroredFileLocation As System.String Dim CopyCustomProperties As System.Boolean Dim value As Component2   value = instance.IMirrorComponents(Plane, InstanceCount, ComponentsToInstance, MirrorCount, ComponentsToMirror, NameCount, MirroredComponentFilenames, RecreateMates, ComponentModifier, ComponentNameModifier, MirroredFileLocation, CopyCustomProperties) ``` | |

| C# |  |
| --- | --- |
| ``` Component2 IMirrorComponents(     System.object Plane,    System.int InstanceCount,    ref Component2 ComponentsToInstance,    System.int MirrorCount,    ref Component2 ComponentsToMirror,    System.int NameCount,    ref System.string MirroredComponentFilenames,    System.bool RecreateMates,    System.int ComponentModifier,    System.string ComponentNameModifier,    System.string MirroredFileLocation,    System.bool CopyCustomProperties ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Component2^ IMirrorComponents(  &   System.Object^ Plane, &   System.int InstanceCount, &   Component2^% ComponentsToInstance, &   System.int MirrorCount, &   Component2^% ComponentsToMirror, &   System.int NameCount, &   System.String^% MirroredComponentFilenames, &   System.bool RecreateMates, &   System.int ComponentModifier, &   System.String^ ComponentNameModifier, &   System.String^ MirroredFileLocation, &   System.bool CopyCustomProperties ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Plane*
:   Plane or planar face about which to mirror the components

*InstanceCount*
:   Number of instances of the components to mirror

*ComponentsToInstance*
:   Array of instances of the [component](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to mirror

*MirrorCount*
:   Number of components to mirror

*ComponentsToMirror*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) to mirror

*NameCount*
:   Number of filenames for the newly created mirrored assemblies or parts

*MirroredComponentFilenames*
:   Array of filenames for the newly created mirrored assemblies or parts

*RecreateMates*
:   True to preserve any mates between the selected components if more than one component is to be mirrored, false to not

*ComponentModifier*
:   Prefix or suffix for the newly mirrored components if MirroredComponentFilenames is not specified, as defined by swMirrorComponentNameModifier\_e

*ComponentNameModifier*
:   String to add to the prefix or suffix of the name of the newly mirrored components if MirroredComponentFilenames is not specified

*MirroredFileLocation*
:   Name of the folder where to store the file of the newly created mirrored components

*CopyCustomProperties*
:   True to copy the custom properties from the selected components to the mirrored components, false to not

#### Return Value

* in-process, unmanaged C++: Pointer to an array of newly created [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html)

* VBA, VB.NET, C#, and C++/CLI: Not supported

See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::IMirrorComponents.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::MirrorComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~MirrorComponents.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0