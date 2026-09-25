<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMacroFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMacroFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMacroFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BaseName*

*ProgId*

*MacroMethods*

*ParamNames*

*ParamTypes*

*ParamValues*

*EditBody*

*Options*

Obsolete. Superseded by [IFeatureManager::InsertMacroFeature3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertMacroFeature3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMacroFeature( _    ByVal BaseName As System.String, _    ByVal ProgId As System.String, _    ByVal MacroMethods As System.Object, _    ByVal ParamNames As System.Object, _    ByVal ParamTypes As System.Object, _    ByVal ParamValues As System.Object, _    ByVal EditBody As Body2, _    ByVal Options As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BaseName As System.String Dim ProgId As System.String Dim MacroMethods As System.Object Dim ParamNames As System.Object Dim ParamTypes As System.Object Dim ParamValues As System.Object Dim EditBody As Body2 Dim Options As System.Integer Dim value As Feature   value = instance.InsertMacroFeature(BaseName, ProgId, MacroMethods, ParamNames, ParamTypes, ParamValues, EditBody, Options) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMacroFeature(     System.string BaseName,    System.string ProgId,    System.object MacroMethods,    System.object ParamNames,    System.object ParamTypes,    System.object ParamValues,    Body2 EditBody,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMacroFeature(  &   System.String^ BaseName, &   System.String^ ProgId, &   System.Object^ MacroMethods, &   System.Object^ ParamNames, &   System.Object^ ParamTypes, &   System.Object^ ParamValues, &   Body2^ EditBody, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BaseName*

*ProgId*

*MacroMethods*

*ParamNames*

*ParamTypes*

*ParamValues*

*EditBody*

*Options*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMacroFeature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)