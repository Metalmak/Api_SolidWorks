<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ChangeSketchPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ChangeSketchPlane Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ChangeSketchPlane Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Config\_opt*
:   Configurations as defined by swInConfigurationOpts\_e

*Config\_names*
:   Array of configuration names

Changes the plane used by a sketch by moving the selected sketch to the selected plane in the specified configurations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ChangeSketchPlane( _    ByVal Config_opt As System.Integer, _    ByVal Config_names As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Config_opt As System.Integer Dim Config_names As System.Object Dim value As System.Boolean   value = instance.ChangeSketchPlane(Config_opt, Config_names) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ChangeSketchPlane(     System.int Config_opt,    System.object Config_names ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ChangeSketchPlane(  &   System.int Config_opt, &   System.Object^ Config_names ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Config\_opt*
:   Configurations as defined by swInConfigurationOpts\_e

*Config\_names*
:   Array of configuration names

#### Return Value

True if the operation succeeds, false if it fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ChangeSketchPlane.

# ![](dotnetimages/collapse.gif)Example

[Change Plane of Sketch (VBA)](Change_Sketch_Plane_Example_VB.htm)

[Change Plane of Sketch (VB.NET)](Change_Sketch_of_Plane_Example_VBNET.htm)

[Change Plane of Sketch (C#)](Change_Sketch_of_Plane_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Every sketch is associated with a plane (for example, a reference plane or a planar face). You must preselect the sketch and the new plane or face before using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::IChangeSketchPlane Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IChangeSketchPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP04, Revision Number 16.4