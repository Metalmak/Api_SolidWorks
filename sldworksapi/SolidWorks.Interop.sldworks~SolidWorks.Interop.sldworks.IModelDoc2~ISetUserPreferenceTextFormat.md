<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ISetUserPreferenceTextFormat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetUserPreferenceTextFormat Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ISetUserPreferenceTextFormat Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceValue*
:   User preference to change as defined in swUserPreferenceTextFormat\_e

*Value*
:   Text format to which to assign the user preference specified in UserPreferenceValue

Obsolete. Superseded by [IModelDocExtension::SetUserPreferenceTextFormat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SetUserPreferenceTextFormat.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetUserPreferenceTextFormat( _    ByVal UserPreferenceValue As System.Integer, _    ByVal Value As TextFormat _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim UserPreferenceValue As System.Integer Dim Value As TextFormat Dim value As System.Boolean   value = instance.ISetUserPreferenceTextFormat(UserPreferenceValue, Value) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ISetUserPreferenceTextFormat(     System.int UserPreferenceValue,    TextFormat Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ISetUserPreferenceTextFormat(  &   System.int UserPreferenceValue, &   TextFormat^ Value ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserPreferenceValue*
:   User preference to change as defined in swUserPreferenceTextFormat\_e

*Value*
:   Text format to which to assign the user preference specified in UserPreferenceValue

#### Return Value

True if the setting is changed successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ISetUserPreferenceTextFormat.

# ![](dotnetimages/collapse.gif)Remarks

This method is

* intended for setting detailing text formats.* equivalent to interactively setting document options in the SOLIDWORKS software.

See System Options and Document Properties for details.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0