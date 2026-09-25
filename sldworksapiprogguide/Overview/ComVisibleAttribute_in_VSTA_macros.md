<!-- source: sldworksapiprogguide/Overview/ComVisibleAttribute_in_VSTA_macros.htm -->

# SOLIDWORKS API Help

# ComVisibleAttribute in VB.NET and C# Macros and Add-ins

VB.NET and C# macros and add-ins must specify a runtime
class attribute, ComVisibleAttribute, when implementing SolidWorks.Interop.swpublished
interfaces.

For example, when defining an object that implements any of the interfaces
in SolidWorks.Interop.swpublished, specify the System.Runtime.InteropServices.ComVisibleAttribute
class attribute on the line before the implementing class. Note the underscore
character at the end of the first line of the VB.NET example.

## VB.NET

<System.Runtime.InteropServices.ComVisibleAttribute(True)>
\_

Public Class clsPropMgr

       Implements
PropertyManagerPage2Handler7

{

## C#

[System.Runtime.InteropServices.ComVisibleAttribute(true)]

public class clsPropMgr : PropertyManagerPage2Handler7

{

Use ComVisibleAttribute in VB.NET and C# macros and add-ins that implement these interfaces:

* IPropertyManagerPage2Handler7
* ISwAddin
* ISwAddinBroker
* ISwCalloutHandler
* ISwColorContour
* ISwComFeature
* ISwManipulatorHandler2
* ISwQuicktip
* ISwUndoAPIHandler