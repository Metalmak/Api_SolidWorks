<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetUserValueIn2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUserValueIn2 Method (IDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html) : SetUserValueIn2 Method (IDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Doc*
:   Document whose units you want to use

*NewValue*
:   Value for this dimension in the units of the Doc argument

*WhichConfigurations*
:   Configurations to set this value in as defined in swSetValueInConfiguration\_e

Sets the value of this dimension in the units of the specified document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetUserValueIn2( _    ByVal Doc As System.Object, _    ByVal NewValue As System.Double, _    ByVal WhichConfigurations As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimension Dim Doc As System.Object Dim NewValue As System.Double Dim WhichConfigurations As System.Integer Dim value As System.Integer   value = instance.SetUserValueIn2(Doc, NewValue, WhichConfigurations) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetUserValueIn2(     System.object Doc,    System.double NewValue,    System.int WhichConfigurations ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetUserValueIn2(  &   System.Object^ Doc, &   System.double NewValue, &   System.int WhichConfigurations ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Doc*
:   Document whose units you want to use

*NewValue*
:   Value for this dimension in the units of the Doc argument

*WhichConfigurations*
:   Configurations to set this value in as defined in swSetValueInConfiguration\_e

#### Return Value

Success indicator as defined in swSetValueReturnStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Dimension::SetUserValueIn2.

# ![](dotnetimages/collapse.gif)Remarks

The WhichConfigs argument is equivalent to the **Change Parameter** dialog in the SOLIDWORKS user interface, which gives the user the option of having the value set in all configurations or the current configuration. If there is one configuration in the part, SOLIDWORKS ignores this argument.

This method allows you to change the value of a read-only dimension. You can use [IDimension::ReadOnly](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~ReadOnly.html) to determine if a dimension is read-only.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html)

[IDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension_members.html)

[IDimension::GetSystemValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetSystemValue3.html)

[IDimension::GetUserValueIn Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetUserValueIn.html)

[IDimension::GetValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetValue3.html)

[IDimension::IGetSystemValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetSystemValue3.html)

[IDimension::IGetUserValueIn2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetUserValueIn2.html)

[IDimension::IGetValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetValue3.html)

[IDimension::ISetSystemValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetSystemValue3.html)

[IDimension::ISetUserValueIn3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetUserValueIn3.html)

[IDimension::ISetValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetValue3.html)

[IDimension::SetSystemValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetSystemValue3.html)

[IDimension::SetValue3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetValue3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 98Plus, datecode 1999005