<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetUserPreferenceToggle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUserPreferenceToggle Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetUserPreferenceToggle Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserPreferenceValue*
:   Value to toggle as defined in swUserPreferenceToggle\_e

*OnFlag*
:   True to toggle the value on, false to toggle the value off

Obsolete. Superseded by [IModelDocExtension::SetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SetUserPreferenceToggle.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetUserPreferenceToggle( _    ByVal UserPreferenceValue As System.Integer, _    ByVal OnFlag As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim UserPreferenceValue As System.Integer Dim OnFlag As System.Boolean Dim value As System.Boolean   value = instance.SetUserPreferenceToggle(UserPreferenceValue, OnFlag) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetUserPreferenceToggle(     System.int UserPreferenceValue,    System.bool OnFlag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetUserPreferenceToggle(  &   System.int UserPreferenceValue, &   System.bool OnFlag ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserPreferenceValue*
:   Value to toggle as defined in swUserPreferenceToggle\_e

*OnFlag*
:   True to toggle the value on, false to toggle the value off

#### Return Value

True if the toggle is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetUserPreferenceToggle.

# ![](dotnetimages/collapse.gif)Example

[Hide or Show All Types (VBA)](Hide_or_Show_All_Types_Example_VB.htm)

[Ignore Feature Colors (VBA)](Ignore_Feature_Colors_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is equivalent to interactively setting document properties in the SOLIDWORKS software. See System Options and Document Properties for details.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0