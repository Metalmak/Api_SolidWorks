<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertIndent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertIndent Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertIndent Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Thickness*
:   Thickness of the indent feature

*Clearance*
:   Distance between the tool body and target body (see **Remarks**)

*Exclude*
:   True to exclude the selections, false to include the selections

*ClrDir*
:   True to leave the direction of clearance as is, false to reverse the direction of the clearance

*Cut*
:   True to cut the target body, false to not

*CutDir*
:   True to reverse the direction of the cut if the tool body is a surface, false to not

Inserts an indent feature using a selected target body and tool body regions.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertIndent( _    ByVal Thickness As System.Double, _    ByVal Clearance As System.Double, _    ByVal Exclude As System.Boolean, _    ByVal ClrDir As System.Boolean, _    ByVal Cut As System.Boolean, _    ByVal CutDir As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Thickness As System.Double Dim Clearance As System.Double Dim Exclude As System.Boolean Dim ClrDir As System.Boolean Dim Cut As System.Boolean Dim CutDir As System.Boolean Dim value As Feature   value = instance.InsertIndent(Thickness, Clearance, Exclude, ClrDir, Cut, CutDir) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertIndent(     System.double Thickness,    System.double Clearance,    System.bool Exclude,    System.bool ClrDir,    System.bool Cut,    System.bool CutDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertIndent(  &   System.double Thickness, &   System.double Clearance, &   System.bool Exclude, &   System.bool ClrDir, &   System.bool Cut, &   System.bool CutDir ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Thickness*
:   Thickness of the indent feature

*Clearance*
:   Distance between the tool body and target body (see **Remarks**)

*Exclude*
:   True to exclude the selections, false to include the selections

*ClrDir*
:   True to leave the direction of clearance as is, false to reverse the direction of the clearance

*Cut*
:   True to cut the target body, false to not

*CutDir*
:   True to reverse the direction of the cut if the tool body is a surface, false to not

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertIndent.

# ![](dotnetimages/collapse.gif)Example

[Insert Indent Feature (C#)](Insert_Indent_Feature_Example_CSharp.htm)

[Insert Indent Feature (VB.NET)](Insert_Indent_Feature_Example_VBNET.htm)

[Insert Indent Feature (VBA)](Insert_Indent_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Prior to calling this method, you must have selected the target body and tool body regions, using these selection marks:

* Target body = 1* Tool body region = 4

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IIndentFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IIndentFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0