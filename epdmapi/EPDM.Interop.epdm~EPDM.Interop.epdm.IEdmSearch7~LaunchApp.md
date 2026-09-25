<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7~LaunchApp.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LaunchApp Method (IEdmSearch7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7.html) : LaunchApp Method (IEdmSearch7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle

*bsDefault*
:   Name of a search form; name of a search favorite if lEdmLaunchSearchFlags contains [EdmLaunchSearchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLaunchSearchFlags.html).Elsf\_DefaultIsAFavorite

*oStartFolderPathOrID*
:   Path or ID of the folder in which the search tool should start looking

*lEdmLaunchSearchFlags*
:   Combination of [EdmLaunchSearchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLaunchSearchFlags.html) bits

Starts the search tool application.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LaunchApp( _    ByVal hParentWnd As System.Integer, _    Optional ByVal bsDefault As System.String, _    Optional ByVal oStartFolderPathOrID As System.Object, _    Optional ByVal lEdmLaunchSearchFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LaunchApp(     System.int hParentWnd,    System.string bsDefault,    System.object oStartFolderPathOrID,    System.int lEdmLaunchSearchFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LaunchApp(  &   System.int hParentWnd, &   System.String^ bsDefault, &   System.Object^ oStartFolderPathOrID, &   System.int lEdmLaunchSearchFlags ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle

*bsDefault*
:   Name of a search form; name of a search favorite if lEdmLaunchSearchFlags contains [EdmLaunchSearchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLaunchSearchFlags.html).Elsf\_DefaultIsAFavorite

*oStartFolderPathOrID*
:   Path or ID of the folder in which the search tool should start looking

*lEdmLaunchSearchFlags*
:   Combination of [EdmLaunchSearchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLaunchSearchFlags.html) bits

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7.html)

[IEdmSearch7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009