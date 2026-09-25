<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGussetFeatureData~SetSupportingFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSupportingFaces Method (IGussetFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGussetFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGussetFeatureData.html) : SetSupportingFaces Method (IGussetFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PFace1*
:   Pointer to the first [IFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) object

*PFace2*
:   Pointer to the second [IFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) object

Sets the two, adjacent, supporting faces for this gusset feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSupportingFaces( _    ByVal PFace1 As Face2, _    ByVal PFace2 As Face2 _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGussetFeatureData Dim PFace1 As Face2 Dim PFace2 As Face2 Dim value As System.Boolean   value = instance.SetSupportingFaces(PFace1, PFace2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSupportingFaces(     Face2 PFace1,    Face2 PFace2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSupportingFaces(  &   Face2^ PFace1, &   Face2^ PFace2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PFace1*
:   Pointer to the first [IFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) object

*PFace2*
:   Pointer to the second [IFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) object

#### Return Value

|
|  |

True if the supporting faces are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See GussetFeatureData::SetSupportingFaces.

# ![](dotnetimages/collapse.gif)See Also

####

[IGussetFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGussetFeatureData.html)

[IGussetFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGussetFeatureData_members.html)

[IGussetFeatureData::GetSupportingFaces Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGussetFeatureData~GetSupportingFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0