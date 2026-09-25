<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentConfigurationName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| ComponentConfigurationName Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : ComponentConfigurationName Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Config*
:   Name of a component configuration in the top-level assembly or an asterisk ("\*") for all component configurations in the top-level assembly (see **Remarks**)

*index*
:   Index number of the component whose configuration name to get

Gets the name of the configuration for the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ComponentConfigurationName( _    ByVal Config As System.String, _    ByVal index As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim Config As System.String Dim index As System.Integer Dim value As System.String   value = instance.ComponentConfigurationName(Config, index) ``` | |

| C# |  |
| --- | --- |
| ``` System.string ComponentConfigurationName(     System.string Config,    System.int index ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ ComponentConfigurationName {    System.String^ get(System.String^ Config, System.int index); } ``` | |

#### Parameters

*Config*
:   Name of a component configuration in the top-level assembly or an asterisk ("\*") for all component configurations in the top-level assembly (see **Remarks**)

*index*
:   Index number of the component whose configuration name to get

#### Property Value

Name of the configuration for the component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::ComponentConfigurationName.

# ![](dotnetimages/collapse.gif)Example

Visual Basic code snippet that shows how to get the names of the components and the names of their component configurations in a top-level assembly configuration named Level1\_Config2:

```
    count = Document.EModelViewControl.ComponentCount("Level1_Config2")
    for index = 0 to count
        componentName = Document.EModelViewControl.ComponentName("Level1_Config2", index)
        configurationName = Document.EModelViewControl.ComponentConfigurationName ("Level1_Config2", index)
        Debug.Print "Component name: " & componentName & " , Component configuration name: " & configurationName
    next
```

# ![](dotnetimages/collapse.gif)Remarks

This property does not get component configuration names for inactive component configurations of a top-level assembly in a SOLIDWORKS document. To get the component configuration names for inactive component configurations of a top-level assembly, you must use an eDrawings file that was published from SOLIDWORKS.

Before calling this property, call:

* [IEModelViewControl::ConfigurationName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ConfigurationName.html) to get the name of a top-level assembly configuration.* [IEModelViewControl::ComponentCount](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentCount.html) to get a valid value for index.* [IEModelViewControl::ComponentName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentName.html) so that you know which component refers to which configuration.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::ComponentState](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentState.html)

[IEModelViewControl::ComponentTransform](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentTransform.html)

[IEModelViewControl::ConfigurationCount](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ConfigurationCount.html)

[IEModelViewControl::CurrentConfigurationIndex](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~CurrentConfigurationIndex.html)

[IEModelViewControl::ShowConfiguration](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ShowConfiguration.html)

[IEModelViewControl::GetSelectedComponentName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~GetSelectedComponentName.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2013 SP0