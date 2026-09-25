<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFormTool2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFormTool2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : CreateFormTool2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OriginX*
:   x coordinate of insertion point

*OriginY*
:   y coordinate of insertion point

Creates a forming tool feature with the specified point of insertion in a sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFormTool2( _    ByVal OriginX As System.Double, _    ByVal OriginY As System.Double _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim OriginX As System.Double Dim OriginY As System.Double Dim value As Feature   value = instance.CreateFormTool2(OriginX, OriginY) ``` | |

| C# |  |
| --- | --- |
| ``` Feature CreateFormTool2(     System.double OriginX,    System.double OriginY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ CreateFormTool2(  &   System.double OriginX, &   System.double OriginY ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OriginX*
:   x coordinate of insertion point

*OriginY*
:   y coordinate of insertion point

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::CreateFormTool2.

# ![](dotnetimages/collapse.gif)Example

[Create Forming Tool (VBA)](Create_Forming_Tool_Example_VB.htm)

[Create Forming Tool (VB.NET)](Create_Forming_Tool_Example_VBNET.htm)

[Create Forming Tool (C#)](Create_Forming_Tool_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html):

1. with Append = True and Mark = 1 to select the stopping face.- (optional) one or more times with Append = True and Mark = 2 to select the faces to remove.

To insert a forming tool from the Design Library, call [IFeatureManager::InsertFormToolFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertFormToolFeature.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0