<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddDisplayStateSpecificRenderMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddDisplayStateSpecificRenderMaterial Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : AddDisplayStateSpecificRenderMaterial Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PRenderMaterial*
:   [Appearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html) to add

*DisplayStateOption*
:   Display states as defined in swDisplayStateOpts\_e

*DisplayStateNames*
:   Names of display states to which to add the appearance

*PWMaterialId1*
:   First ID of appearance

*PWMaterialId2*
:   Second ID of appearance

Adds the specified appearance to the specified display states in the active configuration and returns the IDs assigned to that appearance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDisplayStateSpecificRenderMaterial( _    ByVal PRenderMaterial As RenderMaterial, _    ByVal DisplayStateOption As System.Integer, _    ByVal DisplayStateNames As System.Object, _    ByRef PWMaterialId1 As System.Integer, _    ByRef PWMaterialId2 As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim PRenderMaterial As RenderMaterial Dim DisplayStateOption As System.Integer Dim DisplayStateNames As System.Object Dim PWMaterialId1 As System.Integer Dim PWMaterialId2 As System.Integer Dim value As System.Boolean   value = instance.AddDisplayStateSpecificRenderMaterial(PRenderMaterial, DisplayStateOption, DisplayStateNames, PWMaterialId1, PWMaterialId2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddDisplayStateSpecificRenderMaterial(     RenderMaterial PRenderMaterial,    System.int DisplayStateOption,    System.object DisplayStateNames,    out System.int PWMaterialId1,    out System.int PWMaterialId2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddDisplayStateSpecificRenderMaterial(  &   RenderMaterial^ PRenderMaterial, &   System.int DisplayStateOption, &   System.Object^ DisplayStateNames, &   [Out] System.int PWMaterialId1, &   [Out] System.int PWMaterialId2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PRenderMaterial*
:   [Appearance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html) to add

*DisplayStateOption*
:   Display states as defined in swDisplayStateOpts\_e

*DisplayStateNames*
:   Names of display states to which to add the appearance

*PWMaterialId1*
:   First ID of appearance

*PWMaterialId2*
:   Second ID of appearance

#### Return Value

True if appearance is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::AddDisplayStateSpecificRenderMaterial.

# ![](dotnetimages/collapse.gif)Example

[Add and Delete Appearances from Specific Display States (C#)](Add_and_Delete_Materials_from_Specific_Display_States_Example_CSharp.htm)

[Add and Delete Appearances from Specific Display States (VB.NET)](Add_and_Delete_Materials_from_Specific_Display_States_Example_VBNET.htm)

[Add and Delete Appearances from Specific Display States (VBA)](Add_and_Delete_Materials_from_Specific_Display_States_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::DeleteDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteDisplayStateSpecificRenderMaterial.html)

[IModelDocExtension::IAddDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IAddDisplayStateSpecificRenderMaterial.html)

[IModelDocExtension::IDeleteDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IDeleteDisplayStateSpecificRenderMaterial.html)

[IConfiguration::CreateDisplayState Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IConfiguration~CreateDisplayState.html)

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0