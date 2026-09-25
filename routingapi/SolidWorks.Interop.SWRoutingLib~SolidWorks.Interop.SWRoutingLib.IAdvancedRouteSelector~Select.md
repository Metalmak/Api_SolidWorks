<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector~Select.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| Select Method (IAdvancedRouteSelector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) : Select Method (IAdvancedRouteSelector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*selIndex*
:   Index of the component (fitting, cable, or wire) to select

*append*
:   True appends the selection to the selection list, false replaces the selection list with this selection

*callbackIn*
:   SOLIDWORKS SelectData or NULL

*outputType*
:   Output type as defined by [swAdvancedRouteSelectionOutput\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAdvancedRouteSelectionOutput_e.html)

*selObjName*
:   Array of length 1; contains either the name of the selected component or an empty string (see **Remarks**)

Gets the names of the attached components for the selected component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Select( _    ByVal selIndex As System.Integer, _    ByVal append As System.Boolean, _    ByVal callbackIn As System.Object, _    ByVal outputType As System.Integer, _    ByRef selObjName As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedRouteSelector Dim selIndex As System.Integer Dim append As System.Boolean Dim callbackIn As System.Object Dim outputType As System.Integer Dim selObjName As System.Object Dim value As System.Object   value = instance.Select(selIndex, append, callbackIn, outputType, selObjName) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Select(     System.int selIndex,    System.bool append,    System.object callbackIn,    System.int outputType,    out System.object selObjName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Select(  &   System.int selIndex, &   System.bool append, &   System.Object^ callbackIn, &   System.int outputType, &   [Out] System.Object^ selObjName ) ``` | |

#### Parameters

*selIndex*
:   Index of the component (fitting, cable, or wire) to select

*append*
:   True appends the selection to the selection list, false replaces the selection list with this selection

*callbackIn*
:   SOLIDWORKS SelectData or NULL

*outputType*
:   Output type as defined by [swAdvancedRouteSelectionOutput\_e](SOLIDWORKS.Interop.SWRoutingLib~SOLIDWORKS.Interop.SWRoutingLib.swAdvancedRouteSelectionOutput_e.html)

*selObjName*
:   Array of length 1; contains either the name of the selected component or an empty string (see **Remarks**)

#### Return Value

Array of names of the attached components for the selected component (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedRouteSelector::Select.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedRouteSelector](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Both selObjName and the return value of this method are Variant SafeArrays of BSTRs. See Passing SafeArrays in Visual Basic and Passing SafeArrays in C++ for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html)

[IAdvancedRouteSelector Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS