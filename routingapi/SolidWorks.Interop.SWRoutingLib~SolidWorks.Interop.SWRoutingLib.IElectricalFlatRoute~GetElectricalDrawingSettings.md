<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute~GetElectricalDrawingSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetElectricalDrawingSettings Method (IElectricalFlatRoute) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html) : GetElectricalDrawingSettings Method (IElectricalFlatRoute) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*elecBomTblTmplt*
:   Path and filename of the electrical (ECAD) BOM table template

*cutListTmplt*
:   Path and filename of the cut list table template

*ConnectorTblTmplt*
:   Path and filename of the connector table template

Gets the electrical drawing settings for this flat route.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetElectricalDrawingSettings( _    ByRef elecBomTblTmplt As System.String, _    ByRef cutListTmplt As System.String, _    ByRef ConnectorTblTmplt As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IElectricalFlatRoute Dim elecBomTblTmplt As System.String Dim cutListTmplt As System.String Dim ConnectorTblTmplt As System.String Dim value As System.Integer   value = instance.GetElectricalDrawingSettings(elecBomTblTmplt, cutListTmplt, ConnectorTblTmplt) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetElectricalDrawingSettings(     out System.string elecBomTblTmplt,    out System.string cutListTmplt,    out System.string ConnectorTblTmplt ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetElectricalDrawingSettings(  &   [Out] System.String^ elecBomTblTmplt, &   [Out] System.String^ cutListTmplt, &   [Out] System.String^ ConnectorTblTmplt ) ``` | |

#### Parameters

*elecBomTblTmplt*
:   Path and filename of the electrical (ECAD) BOM table template

*cutListTmplt*
:   Path and filename of the cut list table template

*ConnectorTblTmplt*
:   Path and filename of the connector table template

#### Return Value

0 if successful, 1 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ElectricalFlatRoute::GetElectricalDrawingSettings.

# ![](dotnetimages/collapse.gif)See Also

####

[IElectricalFlatRoute Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute.html)

[IElectricalFlatRoute Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IElectricalFlatRoute_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS