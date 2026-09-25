<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateSaveBodyFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateSaveBodyFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : CreateSaveBodyFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Bodies*
:   :   Array of [solid bodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) to save as parts (See **Remarks)**

*FilePaths*
:   :   Array of paths and filenames of the part documents to which to save Bodies

*AssemName*
:   Path and filename of the assembly document to which to save Bodies

*ConsumeBody*
:   See **Remarks**

*CopyCustomProperty*
:   See **Remarks**

Creates a Save Bodies feature and creates part and assembly documents of the save bodies.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateSaveBodyFeature( _    ByVal Bodies As System.Object, _    ByVal FilePaths As System.Object, _    ByVal AssemName As System.String, _    ByVal ConsumeBody As System.Boolean, _    ByVal CopyCustomProperty As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Bodies As System.Object Dim FilePaths As System.Object Dim AssemName As System.String Dim ConsumeBody As System.Boolean Dim CopyCustomProperty As System.Boolean Dim value As System.Object   value = instance.CreateSaveBodyFeature(Bodies, FilePaths, AssemName, ConsumeBody, CopyCustomProperty) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateSaveBodyFeature(     System.object Bodies,    System.object FilePaths,    System.string AssemName,    System.bool ConsumeBody,    System.bool CopyCustomProperty ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateSaveBodyFeature(  &   System.Object^ Bodies, &   System.Object^ FilePaths, &   System.String^ AssemName, &   System.bool ConsumeBody, &   System.bool CopyCustomProperty ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Bodies*
:   :   Array of [solid bodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) to save as parts (See **Remarks)**

*FilePaths*
:   :   Array of paths and filenames of the part documents to which to save Bodies

*AssemName*
:   Path and filename of the assembly document to which to save Bodies

*ConsumeBody*
:   See **Remarks**

*CopyCustomProperty*
:   See **Remarks**

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::CreateSaveBodyFeature.

# ![](dotnetimages/collapse.gif)Example

[Create Save Bodies Feature and Create an Assembly (VBA)](Create_Save_Bodies_Feature_and_Create_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If any solid bodies in Bodies are invalid, they are skipped/ignored.

| For parameter... | Specify... |
| --- | --- |
| ConsumeBody | VARIANT\_TRUE (-1) to consume all bodies in the original part, VARIANT\_FALSE (0) to not |
| CopyCustomProperty | VARIANT\_TRUE (-1) to copy custom properties to the new parts, VARIANT\_FALSE (0) to not |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ISaveBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0