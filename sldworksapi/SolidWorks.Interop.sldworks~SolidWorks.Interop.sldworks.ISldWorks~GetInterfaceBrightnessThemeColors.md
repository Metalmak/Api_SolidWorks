<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetInterfaceBrightnessThemeColors.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetInterfaceBrightnessThemeColors Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetInterfaceBrightnessThemeColors Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Colors*
:   Array of nine RGB (Red, Green, Blue) decimal values corresponding to the nine color types of the SOLIDWORKS background as defined in swInterfaceBrightnessColor\_e

Gets the theme and colors of the SOLIDWORKS background.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetInterfaceBrightnessThemeColors( _    ByRef Colors As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim Colors As System.Object Dim value As System.Integer   value = instance.GetInterfaceBrightnessThemeColors(Colors) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetInterfaceBrightnessThemeColors(     out System.object Colors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetInterfaceBrightnessThemeColors(  &   [Out] System.Object^ Colors ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Colors*
:   Array of nine RGB (Red, Green, Blue) decimal values corresponding to the nine color types of the SOLIDWORKS background as defined in swInterfaceBrightnessColor\_e

#### Return Value

SOLIDWORKS background theme as defined in swInterfaceBrightnessTheme\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetInterfaceBrightnessThemeColors.

# ![](dotnetimages/collapse.gif)Remarks

A SOLIDWORKS add-in can:

* use this method to determine the current theme and colors of the SOLIDWORKS background.* be notified when the theme and colors in the SOLIDWORKS background change by registering for the [DSldWorksEvents\_InterfaceBrightnessThemeChangeNotifyEventHandler](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_InterfaceBrightnessThemeChangeNotifyEventHandler.html) event.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

ISwHtmlInterface::GetInterfaceBrightnessTheme

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 SP2, Revision Number 24.2