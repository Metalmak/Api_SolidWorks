<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~ImportFromToList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| ImportFromToList Method (IRouteManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : ImportFromToList Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*fromtoListFileName*
:   Pathname of the Excel file (\*.xlsx) containing the from-to list

*componentLibraryFilename*
:   Pathname of a SOLIDWORKS component library in XML format

*cableWireLibraryFileName*
:   Pathname of a SOLIDWORKS cable/wire library in XML format

*useExistingAssembly*
:   True to use an existing assembly, false to start a new assembly

*overwriteData*
:   True to overwrite data, false to insert data; applies only if useExistingAssembly = true

*searchAllSubAssemblies*
:   True to search all sub-assemblies for pre-placed connectors, false to not

Imports electrical connection data (guidelines) using the specified from-to list.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ImportFromToList( _    ByVal fromtoListFileName As System.String, _    ByVal componentLibraryFilename As System.String, _    ByVal cableWireLibraryFileName As System.String, _    ByVal useExistingAssembly As System.Boolean, _    ByVal overwriteData As System.Boolean, _    ByVal searchAllSubAssemblies As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim fromtoListFileName As System.String Dim componentLibraryFilename As System.String Dim cableWireLibraryFileName As System.String Dim useExistingAssembly As System.Boolean Dim overwriteData As System.Boolean Dim searchAllSubAssemblies As System.Boolean Dim value As System.Boolean   value = instance.ImportFromToList(fromtoListFileName, componentLibraryFilename, cableWireLibraryFileName, useExistingAssembly, overwriteData, searchAllSubAssemblies) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ImportFromToList(     System.string fromtoListFileName,    System.string componentLibraryFilename,    System.string cableWireLibraryFileName,    System.bool useExistingAssembly,    System.bool overwriteData,    System.bool searchAllSubAssemblies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ImportFromToList(  &   System.String^ fromtoListFileName, &   System.String^ componentLibraryFilename, &   System.String^ cableWireLibraryFileName, &   System.bool useExistingAssembly, &   System.bool overwriteData, &   System.bool searchAllSubAssemblies ) ``` | |

#### Parameters

*fromtoListFileName*
:   Pathname of the Excel file (\*.xlsx) containing the from-to list

*componentLibraryFilename*
:   Pathname of a SOLIDWORKS component library in XML format

*cableWireLibraryFileName*
:   Pathname of a SOLIDWORKS cable/wire library in XML format

*useExistingAssembly*
:   True to use an existing assembly, false to start a new assembly

*overwriteData*
:   True to overwrite data, false to insert data; applies only if useExistingAssembly = true

*searchAllSubAssemblies*
:   True to search all sub-assemblies for pre-placed connectors, false to not

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::ImportFromToList.

# ![](dotnetimages/collapse.gif)Example

[Import a From-To List Example (C#)](Import_a_From-To_List_Example_CSharp.htm)

[Import a From-To List Example (VB.NET)](Import_a_From-To_List_Example_VBNET.htm)

[Import a From-To List Example (VBA)](Import_a_From-To_List_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

1. In the FeatureManager design tree, select the assembly that contains the route to which to add guidelines.- Call [IRouteManager::EditRoute](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.IRouteManager~EditRoute.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

[IAutoRoute::ConvertGuidelinesToRoute Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~ConvertGuidelinesToRoute.html)

[IAutoRoute::MergeGuidelines Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~MergeGuidelines.html)

[IAutoRoute::SelectGuidelines Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~SelectGuidelines.html)

[IAutoRoute::ShowGuidelines Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAutoRoute~ShowGuidelines.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2011 FCS