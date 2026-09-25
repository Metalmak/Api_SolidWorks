<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IDeleteDisplayStateSpecificRenderMaterial.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDeleteDisplayStateSpecificRenderMaterial Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : IDeleteDisplayStateSpecificRenderMaterial Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IdCount*
:   Number of material IDs

*PWMaterialId1*
:   :   * in-process, unmanaged C++: Pointer to an array of the first IDs of the material to delete

        :   - VBA, VB.NET, C#, and C++/CLI: Not supported

              See In-process Methods for details about this type of method.

*PWMaterialId2*
:   :   * in-process, unmanaged C++: Pointer to an array of the second IDs of the material to delete

        :   - VBA, VB.NET, C#, and C++/CLI: Not supported

              See In-process Methods for details about this type of method.

Deletes the specified materials, using the IDs of the materials, from the active configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IDeleteDisplayStateSpecificRenderMaterial( _    ByVal IdCount As System.Integer, _    ByRef PWMaterialId1 As System.Integer, _    ByRef PWMaterialId2 As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim IdCount As System.Integer Dim PWMaterialId1 As System.Integer Dim PWMaterialId2 As System.Integer Dim value As System.Boolean   value = instance.IDeleteDisplayStateSpecificRenderMaterial(IdCount, PWMaterialId1, PWMaterialId2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IDeleteDisplayStateSpecificRenderMaterial(     System.int IdCount,    ref System.int PWMaterialId1,    ref System.int PWMaterialId2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IDeleteDisplayStateSpecificRenderMaterial(  &   System.int IdCount, &   System.int% PWMaterialId1, &   System.int% PWMaterialId2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IdCount*
:   Number of material IDs

*PWMaterialId1*
:   :   * in-process, unmanaged C++: Pointer to an array of the first IDs of the material to delete

        :   - VBA, VB.NET, C#, and C++/CLI: Not supported

              See In-process Methods for details about this type of method.

    *PWMaterialId2*
    :   :   * in-process, unmanaged C++: Pointer to an array of the second IDs of the material to delete

            :   - VBA, VB.NET, C#, and C++/CLI: Not supported

                  See In-process Methods for details about this type of method.

#### Return Value

True if the materials are deleted, false if not

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call:

* [IModelDocExtension::GetRenderMaterialsCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetRenderMaterialsCount.html) to get the value for IdCount.* [IRenderMaterial::GetMaterialIds](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRenderMaterial~GetMaterialIDs.html) to the get the values for PWMaterialId1 and PWMaterialId2, the IDs of the materials added to the model.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::IAddDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IAddDisplayStateSpecificRenderMaterial.html)

[IModelDocExtension::DeleteDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteDisplayStateSpecificRenderMaterial.html)

[IModelDocExtension::AddDisplayStateSpecificRenderMaterial Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~AddDisplayStateSpecificRenderMaterial.html)

[IRenderMaterial Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRenderMaterial.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0