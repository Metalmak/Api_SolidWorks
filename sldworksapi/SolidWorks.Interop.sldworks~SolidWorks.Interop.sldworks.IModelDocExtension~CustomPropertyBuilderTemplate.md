<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CustomPropertyBuilderTemplate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CustomPropertyBuilderTemplate Property (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : CustomPropertyBuilderTemplate Property (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WeldmentTemplate*
:   True if a weldment part, false if not (see **Remarks**)

Gets or sets the custom property builder template for this part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CustomPropertyBuilderTemplate( _    ByVal WeldmentTemplate As System.Boolean _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim WeldmentTemplate As System.Boolean Dim value As System.String   instance.CustomPropertyBuilderTemplate(WeldmentTemplate) = value   value = instance.CustomPropertyBuilderTemplate(WeldmentTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` System.string CustomPropertyBuilderTemplate(     System.bool WeldmentTemplate ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ CustomPropertyBuilderTemplate {    System.String^ get(System.bool WeldmentTemplate);    void set (System.bool WeldmentTemplate, System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WeldmentTemplate*
:   True if a weldment part, false if not (see **Remarks**)

#### Property Value

File name of the custom property builder template (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::CustomPropertyBuilderTemplate.

# ![](dotnetimages/collapse.gif)Example

```
swModDocExt.CustomPropertyBuilderTemplate(False) = "template.prtprp"
```

```
swModDocExt.CustomPropertyBuilderTemplate(True) = "templateWeld2.wldprp"
```

# ![](dotnetimages/collapse.gif)Remarks

If WeldmentTemplate is:

* True, then this property gets or sets **\*.wldprp**.* False, then this property gets or sets **\*.prtprp**.

All custom property builder templates are stored in the file location specified in **Tools > Options > File Locations > Custom Property Files**.

This property corresponds to the setting in the Template Options dialog that appears when you click on the button next to More Properties in the Custom Properties task pane. When you create a custom property layout, a template is created. The button is activated for parts and weldments only after a custom properties tab layout is created. The weldment custom property template (**\*.wldprp**) can be created or modified only if a cut list item is selected in the Cut list folder.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0