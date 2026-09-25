<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2~ReverseFaceNormal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReverseFaceNormal Property (ISimpleFilletFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISimpleFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html) : ReverseFaceNormal Property (ISimpleFilletFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WhichFaceList*
:   Face for Reverse Face Normal option as defined in swSimpleFilletWhichFaces\_e

Gets or sets the Reverse Face Normal option when creating a face fillet between surface bodies.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ReverseFaceNormal( _    ByVal WhichFaceList As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISimpleFilletFeatureData2 Dim WhichFaceList As System.Integer Dim value As System.Boolean   instance.ReverseFaceNormal(WhichFaceList) = value   value = instance.ReverseFaceNormal(WhichFaceList) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReverseFaceNormal(     System.int WhichFaceList ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ReverseFaceNormal {    System.bool get(System.int WhichFaceList);    void set (System.int WhichFaceList, System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WhichFaceList*
:   Face for Reverse Face Normal option as defined in swSimpleFilletWhichFaces\_e

#### Property Value

True if the Reverse Face Normal option is enabled, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SimpleFilletFeatureData2::ReverseFaceNormal.

# ![](dotnetimages/collapse.gif)Example

See [ISimpleFilletFeatureData2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISimpleHoleFeatureData2.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ISimpleFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html)

[ISimpleFilletFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0