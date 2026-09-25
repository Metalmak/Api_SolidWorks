<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| ComponentName Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : ComponentName Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Config*
:   Name of the configuration in which the component exists or an empty string ("") or an asterisk ("\*") (see Remarks)

*index*
:   Index number of the component to get

Gets the name of the component in the specified configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ComponentName( _    ByVal Config As System.String, _    ByVal index As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim Config As System.String Dim index As System.Integer Dim value As System.String   value = instance.ComponentName(Config, index) ``` | |

| C# |  |
| --- | --- |
| ``` System.string ComponentName(     System.string Config,    System.int index ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ ComponentName {    System.String^ get(System.String^ Config, System.int index); } ``` | |

#### Parameters

*Config*
:   Name of the configuration in which the component exists or an empty string ("") or an asterisk ("\*") (see Remarks)

*index*
:   Index number of the component to get

#### Property Value

Name of the component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::ComponentName.

# ![](dotnetimages/collapse.gif)Example

Visual Basic code snippet that shows how to get the names of the components and the names of their component configurations in a top-level assembly configuration named Level1\_Config2:

```
    count = Document.EModelViewControl.ComponentCount("Level1_Config2")
    for index = 0 to count
        componentName = Document.EModelViewControl.ComponentName("Level1_Config2", index)
        configurationName = Document.EModelViewControl.ComponentConfigurationName ("Level1_Config2", index)
        Debug.Print "Component name: " & componentName & " , Component configuration name: " & configurationName
    next
```

# ![](dotnetimages/collapse.gif)Remarks

This property does not get component names for inactive component configurations of a top-level assembly in a SOLIDWORKS document. To get the component names for inactive component configurations of a top-level assembly, you must use an eDrawings file that was published from SOLIDWORKS.

Passing an:

* Empty string ("") to Config gets the name of the component at the specified index from the components in the active configuration.

  * Asterisk ("\*") to Config gets the name of the component at the specified index from the components in all configurations.

You can also call [IEModelViewControl::ConfigurationName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ConfigurationName.html) to get the name of a configuration.

Before calling this property call [IEModelViewControl::ComponentCount](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ConfigurationCount.html) to get a valid value for Index.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::ComponentConfigurationName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentConfigurationName.html)

[IEModelViewControl::ComponentCount](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentCount.html)

[IEModelViewControl::ComponentState](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentState.html)

[IEModelViewControl::ComponentTransform](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ComponentTransform.html)

[IEModelViewControl::GetSelectedComponentName](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~GetSelectedComponentName.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0