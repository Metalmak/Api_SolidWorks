<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DimXpertManager.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DimXpertManager Property (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : DimXpertManager Property (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Configuration*
:   Name of the configuration for which to retrieve the DimXpert schema

*CreateSchema*
:   True to create DimXpert schema if it does not already exist; false otherwise

Gets the DimXpert schema for this configuration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property DimXpertManager( _    ByVal Configuration As System.String, _    ByVal CreateSchema As System.Boolean _ ) As DimXpertManager ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Configuration As System.String Dim CreateSchema As System.Boolean Dim value As DimXpertManager   value = instance.DimXpertManager(Configuration, CreateSchema) ``` | |

| C# |  |
| --- | --- |
| ``` DimXpertManager DimXpertManager(     System.string Configuration,    System.bool CreateSchema ) {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property DimXpertManager^ DimXpertManager {    DimXpertManager^ get(System.String^ Configuration, System.bool CreateSchema); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Configuration*
:   Name of the configuration for which to retrieve the DimXpert schema

*CreateSchema*
:   True to create DimXpert schema if it does not already exist; false otherwise

#### Property Value

[IDimXpertManager](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimXpertManager.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::DimXpertManager.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpertManager Info (VBA)](Get_DimXpertManager_Info_Example_VB.htm)

[Get DimXpertManager Info (VB.NET)](Get_DimXpertManager_Info_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface retrieves the DimXpert schema information for opened parts which can be accessed in SOLIDWORKS via either the DimXpertManager tab of the Management Panel or the DimXpert tab of the CommandManager.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0