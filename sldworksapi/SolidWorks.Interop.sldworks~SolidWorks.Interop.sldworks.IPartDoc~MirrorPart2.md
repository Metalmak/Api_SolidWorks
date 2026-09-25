<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~MirrorPart2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MirrorPart2 Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : MirrorPart2 Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BreakLink*
:   True to break the link to the original part, false to not

*Options*
:   Insertion options as defined in swMirrorPartOptions\_e

*ResultPart*
:   [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html)

Creates a new part document that mirrors this part about a selected reference plane or planar face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MirrorPart2( _    ByVal BreakLink As System.Boolean, _    ByVal Options As System.Integer, _    ByRef ResultPart As ModelDoc2 _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim BreakLink As System.Boolean Dim Options As System.Integer Dim ResultPart As ModelDoc2 Dim value As Feature   value = instance.MirrorPart2(BreakLink, Options, ResultPart) ``` | |

| C# |  |
| --- | --- |
| ``` Feature MirrorPart2(     System.bool BreakLink,    System.int Options,    out ModelDoc2 ResultPart ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ MirrorPart2(  &   System.bool BreakLink, &   System.int Options, &   [Out] ModelDoc2^ ResultPart ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BreakLink*
:   True to break the link to the original part, false to not

*Options*
:   Insertion options as defined in swMirrorPartOptions\_e

*ResultPart*
:   [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html)

#### Return Value

[IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::MirrorPart2.

# ![](dotnetimages/collapse.gif)Example

[Get Mirror Part Information (VBA)](Get_Mirror_Part_Information_Example_VB.htm)

[Get Mirror Part Information (VB.NET)](Get_Mirror_Part_Information_Example_VBNET.htm)

[Get Mirror Part Information (C#)](Get_Mirror_Part_Information_Example_CSharp.htm)

[Mirror Sheet-metal Part (C#)](Mirror_Sheet-metal_Part_Example_CSharp.htm)

[Mirror Sheet-metal Part (VB.NET)](Mirror_Sheet-metal_Part_Example_VBNET.htm)

[Mirror Sheet-metal Part (VBA)](Mirror_Sheet-metal_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must select a reference plane or planar face about which to mirror this part.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IMirrorPartFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorPartFeatureData.html)

[IPartDoc::InsertMirrorAll Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertMirrorAll.html)

[IPartDoc::MirrorFeature Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~MirrorFeature.html)

[IFeatureManager::InsertMirrorFeature2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMirrorFeature2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0