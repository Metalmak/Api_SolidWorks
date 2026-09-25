<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetWhatsWrong.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetWhatsWrong Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetWhatsWrong Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Features*
:   Array of features in the What's Wrong dialog

*ErrorCodes*
:   Array of error codes corresponding to the features in the What's Wrong dialog as defined in swFeatureError\_e

*Warnings*
:   :   Array of Booleans corresponding to the features in the What's Wrong dialog indicating whether SOLIDWORKS detected a What's Wrong item as a warning; true if SOLIDWORKS detected a What's Wrong item as a warning, false if not

Gets the What's Wrong dialog information for this model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetWhatsWrong( _    ByRef Features As System.Object, _    ByRef ErrorCodes As System.Object, _    ByRef Warnings As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Features As System.Object Dim ErrorCodes As System.Object Dim Warnings As System.Object Dim value As System.Boolean   value = instance.GetWhatsWrong(Features, ErrorCodes, Warnings) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetWhatsWrong(     out System.object Features,    out System.object ErrorCodes,    out System.object Warnings ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetWhatsWrong(  &   [Out] System.Object^ Features, &   [Out] System.Object^ ErrorCodes, &   [Out] System.Object^ Warnings ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Features*
:   Array of features in the What's Wrong dialog

*ErrorCodes*
:   Array of error codes corresponding to the features in the What's Wrong dialog as defined in swFeatureError\_e

*Warnings*
:   :   Array of Booleans corresponding to the features in the What's Wrong dialog indicating whether SOLIDWORKS detected a What's Wrong item as a warning; true if SOLIDWORKS detected a What's Wrong item as a warning, false if not

#### Return Value

True if this method runs successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetWhatsWrong.

# ![](dotnetimages/collapse.gif)Example

[Get What's Wrong (C#)](Get_What%27s_Wrong_Example_CSharp.htm)

[Get What's Wrong (VB.NET)](Get_What%27s_Wrong_Example_VBNET.htm)

[Get What's Wrong (VBA)](Get_What%27s_Wrong_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetWhatsWrongCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetWhatsWrongCount.html)

[IFeature::GetErrorCode2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetErrorCode2.html)

[IMacroFeatureData::Provider Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~Provider.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP3, Revision Number 17.3