<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~HideBubbleTooltip.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| HideBubbleTooltip Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : HideBubbleTooltip Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Hides the bubble ToolTip displayed by [ISldWorks::ShowBubbleTooltipAt2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~ShowBubbleTooltipAt2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub HideBubbleTooltip() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks   instance.HideBubbleTooltip() ``` | |

| C# |  |
| --- | --- |
| ``` void HideBubbleTooltip() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void HideBubbleTooltip(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::HideBubbleTooltip.

# ![](dotnetimages/collapse.gif)Example

The following examples show how to display and hide a bubble ToolTip. Click a link to jump to the example in that programming language.

* [C#](#CSharp)* [VB.NET](#VBNET)* [VBA](#VBA)

**C#**

//--------------------------------------------

// Preconditions: SOLIDWORKS is running.

// Postconditions:

// (1) Bubble ToolTip is shown.

// (2) Bubble ToolTip is hidden.

//--------------------------------------------

using

 SOLIDWORKS.Interop.sldworks;

using

 SOLIDWORKS.Interop.swconst;

using

 System;

namespace

 ShowBubbleToolTipAt2SldWorksCSharp.csproj

{

    public partial class SOLIDWORKSMacro

    {

        public void Main()

        {

           // Show bubble ToolTip

           swApp.**ShowBubbleTooltipAt2**(300, 400, (

int)swArrowPosition.swArrowLeftTop, "Sample Bubble Tooltip", "Message of Sample Bubble ToolTip", (int)swBitMaps.swBitMapUserDefined, "C:\\Program Files\\SOLIDWORKS Corp\\SOLIDWORKS\\data\\user macro icons\\questionmark.bmp", "", 0, (int)swLinkString.swLinkStringNone, "", "");

        // 1. Insert a breakpoint at next command.

        // 2. Examine the SOLIDWORKS graphics area to see the bubble ToolTip.

        // 3. Toggle the breakpoint to hide the bubble ToolTip.

        swApp.HideBubbleTooltip();

        }

        /// <summary>

        /// The SldWorks swApp variable is pre-assigned for you.         /// </summary>         public SldWorks swApp;

    }

}

**VB.NET**

'--------------------------------------------

' Preconditions: SOLIDWORKS is running.

' Postconditions:

'   (1) Bubble ToolTip is shown.

'   (2) Bubble ToolTip is hidden.

'--------------------------------------------

Imports

 SOLIDWORKS.Interop.sldworks

Imports

 SOLIDWORKS.Interop.swconst

Imports

 System

Partial Class SOLIDWORKSMacro

Public Sub main()

    ' Show bubble ToolTip

    swApp.**ShowBubbleTooltipAt2**(300, 400, swArrowPosition.swArrowLeftTop, "Sample Bubble Tooltip", "Message of Sample Bubble ToolTip", swBitMaps.swBitMapUserDefined, "C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS\data\user macro icons\questionmark.bmp", "", 0, swLinkString.swLinkStringNone, "", "")

    Stop

    swApp.HideBubbleTooltip()

End Sub

    ''' <summary>

    ''' The SldWorks swApp variable is pre-assigned for you.

    ''' </summary>

    Public swApp As SldWorks

End Class

**VBA**

'--------------------------------------------
' Preconditions: SOLIDWORKS is running
'
' Postconditions:

'       (1) Bubble ToolTip is shown.

'       (2) Bubble ToolTip is hidden.
'--------------------------------------------

Option Explicit

Sub main()

    Dim swApp As SldWorks.SldWorks
    Set swApp = Application.SldWorks

    ' Show Bubble ToolTip
    swApp.**ShowBubbleTooltipAt2** 300, 400, swArrowLeftTop, "Sample Bubble Tooltip", "Message of Sample Bubble ToolTip", swBitMapUserDefined, "C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS\data\user macro icons\questionmark.bmp", "", 0, swLinkStringNone, "", ""

    Stop

    swApp.HideBubbleTooltip

    End Sub

'--------------------------------------------

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0