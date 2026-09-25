<!-- source: sldworksapiprogguide/Overview/Quick_Tips_and_Bubble_ToolTips.htm -->

# SOLIDWORKS API Help

# Quick Tips and Bubble ToolTips

Typically an add-in's Quick Tips tells a user how to
use the add-in application from start to finish. Creating Quick Tips and
Bubble ToolTips for an add-in requires:

* [Add-in application](#Add-in) to create
  a copy of the Quick Tips interface
* [Each HTML page of the add-in's
  Quick Tips](#HTML) to create a copy of Quick Tips HTML object

## Add-in application

1. Implements a copy of the Quick Tips interface,
   ISwQuickTip,
   which defines the add-in's Quick Tips environment.
2. Creates a copy of the Quick Tips interface using
   ISldWorks::InstallQuickTipGuide

   When an add-in application implements a copy of the Quick Tips interface,
   the SOLIDWORKS application adds a selection to its SOLIDWORKS Help menu
   indicating the existence of that add-in's Quick Tips.

By default, the SOLIDWORKS Quick Tips is
the active Quick Tips. When a user selects an add-in's Quick Tips on the
SOLIDWORKS Help menu, that add-in's Quick Tips becomes active and the
SOLIDWORKS Quick Tips becomes inactive. If a user clicks the Quick Tips
button on the SOLIDWORKS status bar, the SOLIDWORKS Quick Tips becomes
active and any active add-in's Quick Tips becomes inactive. Only one application's
Quick Tips can be active at any one time.

Because an add-in does not know whether or
not its Quick Tips window is active, the add-in should assume that it
is active. The state of the add-in application determines which HTML page
of its Quick Tips is displayed.

3. Calls ISwQuickTip::AppState
   to tell the Quick Tips interface that the state of the add-in application
   has changed. Examples of SOLIDWORKS states are:

1. Create a part.
2. Create a sketch.
3. Create an extrusion.

4. Calls ISldWorks::RefreshQuickTipWindow,
   which causes the SOLIDWORKS application to request a new URL to display
   in the Quick Tips window. The new URL is then returned to the SOLIDWORKS
   application and displayed in the Quick Tips window.
5. When the add-in application
   is closing, callsISldWorks::UnInstallQuickTipGuide
   to uninstall
   the add-in's Quick Tips.

[Back to top](#Top)

## Each Quick Tips HTML page

1. Must specify the correct background color of the
   Quick Tips HTML page as follows:

<style>

body

   {

   background-color:
#ffffe1;

   }

</style>

2. Creates a copy of ISwHtmlInterface, which defines
   the add-in's Quick Tips environment for that HTML page.
3. Calls ISwHtmlInterface::ShowBubbleToolTipAt
   or ISwHtmlInterface::ShowBubbleTooltip,
   which displays a Bubble ToolTip and causes a toolbar or toolbar buttons
   to flash, when a user clicks a link on the Quick Tips HTML page.