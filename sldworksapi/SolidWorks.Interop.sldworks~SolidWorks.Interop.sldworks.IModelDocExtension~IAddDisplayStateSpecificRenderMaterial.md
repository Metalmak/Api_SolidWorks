<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IAddDisplayStateSpecificRenderMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAddDisplayStateSpecificRenderMaterial Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : IAddDisplayStateSpecificRenderMaterial Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PRenderMaterial*
:   [Material](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial.html) to add

*DisplayStateOption*
:   Display states as defined in swDisplayStateOpts\_e

*DisplayStateCount*
:   Number of display states (see **Remarks**)

*DisplayStateNames*
:   * in-process, unmanaged C++: Pointer to an array of the names of the display states to which to add material* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*PWMaterialId1*
:   First ID of material

*PWMaterialId2*
:   Second ID of material

Adds the specified material to the specified display states in the active configuration and returns the IDs assigned to that material.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IAddDisplayStateSpecificRenderMaterial( _    ByVal PRenderMaterial As RenderMaterial, _    ByVal DisplayStateOption As System.Integer, _    ByVal DisplayStateCount As System.Integer, _    ByRef DisplayStateNames As System.String, _    ByRef PWMaterialId1 As System.Integer, _    ByRef PWMaterialId2 As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim PRenderMaterial As RenderMaterial Dim DisplayStateOption As System.Integer Dim DisplayStateCount As System.Integer Dim DisplayStateNames As System.String Dim PWMaterialId1 As System.Integer Dim PWMaterialId2 As System.Integer Dim value As System.Boolean   value = instance.IAddDisplayStateSpecificRenderMaterial(PRenderMaterial, DisplayStateOption, DisplayStateCount, DisplayStateNames, PWMaterialId1, PWMaterialId2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IAddDisplayStateSpecificRenderMaterial(     RenderMaterial PRenderMaterial,    System.int DisplayStateOption,    System.int DisplayStateCount,    ref System.string DisplayStateNames,    out System.int PWMaterialId1,    out System.int PWMaterialId2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IAddDisplayStateSpecificRenderMaterial(  &   RenderMaterial^ PRenderMaterial, &   System.int DisplayStateOption, &   System.int DisplayStateCount, &   System.String^% DisplayStateNames, &   [Out] System.int PWMaterialId1, &   [Out] System.int PWMaterialId2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PRenderMaterial*
:   [Material](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial.html) to add

*DisplayStateOption*
:   Display states as defined in swDisplayStateOpts\_e

*DisplayStateCount*
:   Number of display states (see **Remarks**)

*DisplayStateNames*
:   * in-process, unmanaged C++: Pointer to an array of the names of the display states to which to add material* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

*PWMaterialId1*
:   First ID of material

*PWMaterialId2*
:   Second ID of material

#### Return Value

True if material is added, false if not

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IConfiguration::GetDisplayStatesCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration~GetDisplayStatesCount.html) to get DisplayStateCount.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::IDeleteDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IDeleteDisplayStateSpecificRenderMaterial.html)

[IModelDocExtension::AddDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddDisplayStateSpecificRenderMaterial.html)

[IModelDocExtension::DeleteDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteDisplayStateSpecificRenderMaterial.html)

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0