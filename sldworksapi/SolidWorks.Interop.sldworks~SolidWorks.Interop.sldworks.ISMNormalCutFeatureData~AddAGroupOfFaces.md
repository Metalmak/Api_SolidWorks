<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData~AddAGroupOfFaces.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddAGroupOfFaces Method (ISMNormalCutFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISMNormalCutFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData.html) : AddAGroupOfFaces Method (ISMNormalCutFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FaceArray*
:   Array of cut-extrude [faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

*Error*
:   Error code as defined in swSMNormalCutError\_e

Obsolete. See [ISMNormalCutFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub AddAGroupOfFaces( _    ByVal FaceArray As System.Object, _    ByRef Error As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISMNormalCutFeatureData Dim FaceArray As System.Object Dim Error As System.Integer   instance.AddAGroupOfFaces(FaceArray, Error) ``` | |

| C# |  |
| --- | --- |
| ``` void AddAGroupOfFaces(     System.object FaceArray,    out System.int Error ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddAGroupOfFaces(  &   System.Object^ FaceArray, &   [Out] System.int Error ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FaceArray*
:   Array of cut-extrude [faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

*Error*
:   Error code as defined in swSMNormalCutError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SMNormalCutFeatureData::AddAGroupOfFaces.

# ![](dotnetimages/collapse.gif)Example

See the [IFeatureManager::AddSMNormalCutType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~AddSMNormalCutType.html) example.

# ![](dotnetimages/collapse.gif)Remarks

FaceArray contains the non-normal side walls of a cut in a sheet metal part.

# ![](dotnetimages/collapse.gif)See Also

####

[ISMNormalCutFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData.html)

[ISMNormalCutFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData_members.html)

[ISMNormalCutFeatureData::RemoveAGroupOfFaces Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData~RemoveAGroupOfFaces.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0