<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_InterfaceBrightnessThemeChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_InterfaceBrightnessThemeChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_InterfaceBrightnessThemeChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ThemeType*
:   SOLIDWORKS background as defined in swInterfaceBrightnessTheme\_e

*Colors*
:   Array of RGB (Red, Green, Blue) decimal values (see **Remarks**)

Notifies an add-in when the SOLIDWORKS background changes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_InterfaceBrightnessThemeChangeNotifyEventHandler( _    ByVal ThemeType As System.Integer, _    ByRef Colors As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_InterfaceBrightnessThemeChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_InterfaceBrightnessThemeChangeNotifyEventHandler(     System.int ThemeType,    ref System.object Colors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_InterfaceBrightnessThemeChangeNotifyEventHandler(  &   System.int ThemeType, &   System.Object^% Colors ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ThemeType*
:   SOLIDWORKS background as defined in swInterfaceBrightnessTheme\_e

*Colors*
:   Array of RGB (Red, Green, Blue) decimal values (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InterfaceBrightnessThemeChangeNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Example

[Add Shortcut Menus to Add-ins (VB.NET)](Add_Shortcut_Menus_to_Add-ins_VBNET.htm)

[Add Shortcut Menus to Add-ins (C#)](Add_Shortcut_Menus_to_Add-ins_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The Colors array is indexed by swInterfaceBrightnessColor\_e.

To get the SOLIDWORKS background:

* theme, use ISwHtmlInterface::GetInterfaceBrightnessTheme.* theme and colors, [ISldWorks::GetInterfaceBrightnessThemeColors](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetInterfaceBrightnessThemeColors.html).

If developing a C++ application, use swAppInterfaceBrightnessThemeChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 SP1, Revision Number 24.1