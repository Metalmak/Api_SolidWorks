<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPartialEdgeFilletData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPartialEdgeFilletData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to partial fillet/chamfer properties.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IPartialEdgeFilletData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartialEdgeFilletData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IPartialEdgeFilletData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IPartialEdgeFilletData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartialEdgeFilletData.

# ![](dotnetimages/collapse.gif)Example

'=====================================================
'Preconditions:
'1. Open *Public\_documents***\samples\tutorial\api\Block20.sldprt**.
'2. Open an Immediate window.
'
'Postconditions:
'1. Creates **Chamfer1**.
'2. **Chamfer1** contains two partial chamfers.
'3. Inspect the Immediate window.
'
'NOTE: Because the model is used elsewhere, do not save changes to it.
'======================================================

Option Explicit
Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim swFeatMgr As SldWorks.FeatureManager
Dim swSelMgr As SldWorks.SelectionMgr
Dim swFeat As SldWorks.Feature
Dim swFilletData As SldWorks.SimpleFilletFeatureData2
Dim PartialEdgeAFilletData As SldWorks.PartialEdgeFilletData
Dim PartialEdgeBFilletData As SldWorks.PartialEdgeFilletData
Dim filletItemA As SldWorks.Edge
Dim filletItemB As SldWorks.Edge
Dim swFeatDataObj As Object
Dim boolstatus As Boolean
Dim errorCode As Long
Dim warning As Boolean
Sub main()

    Set swApp = Application.SldWorks
    Set swModel = swApp.ActiveDoc
    Set swFeatMgr = swModel.FeatureManager
    Set swSelMgr = swModel.SelectionManager

    ' Create the fillet feature data object to be a simple fillet type
    Set swFeatDataObj = swFeatMgr.**CreateDefinition**(swFmFillet)
    Set swFilletData = swFeatDataObj

    ' Initilize the feature type to be a constant radius fillet
    swFilletData.**Initialize** swConstRadiusFillet

    ' Specialize the feature type to be a chamfer
    swFilletData.**ConicTypeForCrossSectionProfile** = swFeatureFilletConicRhoZeroChamfer

    swFilletData.**OverflowType** = swFilletOverFlowType\_Default
    swFilletData.**DefaultRadius** = 0.01

    ' Select two edges to partially chamfer
    boolstatus = swModel.Extension.SelectByRay(-6.27751435901871E-02, 3.95396450382464E-02, 6.03865270420556E-04, 0.156569748366562, -0.551708952719479, -0.81920885333693, 1.1220164860728E-03, 1, False, 1, 0)
    boolstatus = swModel.Extension.SelectByRay(6.44200432014657E-02, 0.039572847309671, 1.30368065144353E-02, 0.156569748366562, -0.551708952719479, -0.81920885333693, 1.1220164860728E-03, 1, True, 1, 0)

    Set filletItemA = swSelMgr.GetSelectedObject6(1, -1)
    Set filletItemB = swSelMgr.GetSelectedObject6(2, -1)

    swFilletData.**EnablePartialEdgeParameters** = True
    Set PartialEdgeAFilletData = swFilletData.**GetPartialEdgeFilletData**(filletItemA)
    PartialEdgeAFilletData.**SetPartialFilletParameters**(True, swPartialEdgeDistanceOffset, 0.01, Nothing, swPartialEdgeDistanceOffset, 0.03, Nothing)
    Set PartialEdgeBFilletData = swFilletData.**GetPartialEdgeFilletData**(filletItemB)
    PartialEdgeBFilletData.**SetPartialFilletParameters**(False, swPartialEdgeDistanceOffset, 0.01, Nothing, swPartialEdgeDistanceOffset, 0.03, Nothing)

    Set swFeat = swFeatMgr.**CreateFeature**(swFilletData)

    errorCode = swFeat.**GetErrorCode2**(warning)

End Sub

# ![](dotnetimages/collapse.gif)Example

[Create Partial Chamfer (C#)](Create_Partial_Chamfer_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IFeature.GetErrorCode2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetErrorCode2.html) after creating the partial edge fillet feature to see if anything is wrong with the new feature.

For more information, see the **Partial Edge Parameters** section of the **Constant Size Fillets** topic in the SOLIDWORKS user-interface help.

# ![](dotnetimages/collapse.gif)Accessors

[ISimpleFilletFeatureData2::GetPartialEdgeFilletData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2~GetPartialEdgeFilletData.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[PartialEdgeFilletData](SWObjectModel.pdf#PartialEdgeFilletData)

# ![](dotnetimages/collapse.gif)See Also

####

[IPartialEdgeFilletData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartialEdgeFilletData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)