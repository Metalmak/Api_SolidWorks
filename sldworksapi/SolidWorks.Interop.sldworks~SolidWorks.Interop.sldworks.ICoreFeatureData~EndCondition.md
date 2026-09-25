<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~EndCondition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EndCondition Property (ICoreFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html) : EndCondition Property (ICoreFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Direction of end conditions as defined in swCoreFeatureDirection\_e

Gets or sets the end condition in the specified direction for this core feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EndCondition( _    ByVal Index As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICoreFeatureData Dim Index As System.Integer Dim value As System.Integer   instance.EndCondition(Index) = value   value = instance.EndCondition(Index) ``` | |

| C# |  |
| --- | --- |
| ``` System.int EndCondition(     System.int Index ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int EndCondition {    System.int get(System.int Index);    void set (System.int Index, System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Direction of end conditions as defined in swCoreFeatureDirection\_e

#### Property Value

Type of end conditions as defined in swEndConditions\_e (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CoreFeatureData::EndCondition.

# ![](dotnetimages/collapse.gif)Example

[Get Core Feature Data (C#)](Get_Core_Feature_Example_CSharp.htm)

[Get Core Feature Data (VB.NET)](Get_Core_Feature_Example_VBNET.htm)

[Get Core Feature Data (VBA)](Get_Core_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Valid end conditions are swEndConditions\_e:

* swEndCondBlind* swEndCondThroughAll* swEndCondThroughNext

# ![](dotnetimages/collapse.gif)See Also

####

[ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html)

[ICoreFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0