<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IInsertMacroFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IInsertMacroFeature Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IInsertMacroFeature Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CmdFile*

*CmdModule*

*CmdProcedure*

*ParamCount*

*ParamNames*

*ParamTypes*

*ParamValues*

*PmFile*

*PmModule*

*PmProcedure*

Obsolete. Superseded by [IFeatureManager::IInsertMacroFeature3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~IInsertMacroFeature3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IInsertMacroFeature( _    ByVal CmdFile As System.String, _    ByVal CmdModule As System.String, _    ByVal CmdProcedure As System.String, _    ByVal ParamCount As System.Integer, _    ByRef ParamNames As System.String, _    ByRef ParamTypes As System.Integer, _    ByRef ParamValues As System.String, _    ByVal PmFile As System.String, _    ByVal PmModule As System.String, _    ByVal PmProcedure As System.String _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim CmdFile As System.String Dim CmdModule As System.String Dim CmdProcedure As System.String Dim ParamCount As System.Integer Dim ParamNames As System.String Dim ParamTypes As System.Integer Dim ParamValues As System.String Dim PmFile As System.String Dim PmModule As System.String Dim PmProcedure As System.String Dim value As Feature   value = instance.IInsertMacroFeature(CmdFile, CmdModule, CmdProcedure, ParamCount, ParamNames, ParamTypes, ParamValues, PmFile, PmModule, PmProcedure) ``` | |

| C# |  |
| --- | --- |
| ``` Feature IInsertMacroFeature(     System.string CmdFile,    System.string CmdModule,    System.string CmdProcedure,    System.int ParamCount,    ref System.string ParamNames,    ref System.int ParamTypes,    ref System.string ParamValues,    System.string PmFile,    System.string PmModule,    System.string PmProcedure ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ IInsertMacroFeature(  &   System.String^ CmdFile, &   System.String^ CmdModule, &   System.String^ CmdProcedure, &   System.int ParamCount, &   System.String^% ParamNames, &   System.int% ParamTypes, &   System.String^% ParamValues, &   System.String^ PmFile, &   System.String^ PmModule, &   System.String^ PmProcedure ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CmdFile*

*CmdModule*

*CmdProcedure*

*ParamCount*

*ParamNames*

*ParamTypes*

*ParamValues*

*PmFile*

*PmModule*

*PmProcedure*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::IInsertMacroFeature.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)