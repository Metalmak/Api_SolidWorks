<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark~SetExtendedLength.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetExtendedLength Method (ICenterMark) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html) : SetExtendedLength Method (ICenterMark) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*GroupID*
:   Instance of center mark (see Remarks)

*HandleID*
:   Center mark handle ID as defined by swCenterMarkHandle\_e

*ExtendedLength*
:   Extended length of HandleID

Sets the extended length of this center mark.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetExtendedLength( _    ByVal GroupID As System.Integer, _    ByVal HandleID As System.Integer, _    ByVal ExtendedLength As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICenterMark Dim GroupID As System.Integer Dim HandleID As System.Integer Dim ExtendedLength As System.Double Dim value As System.Boolean   value = instance.SetExtendedLength(GroupID, HandleID, ExtendedLength) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetExtendedLength(     System.int GroupID,    System.int HandleID,    System.double ExtendedLength ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetExtendedLength(  &   System.int GroupID, &   System.int HandleID, &   System.double ExtendedLength ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*GroupID*
:   Instance of center mark (see Remarks)

*HandleID*
:   Center mark handle ID as defined by swCenterMarkHandle\_e

*ExtendedLength*
:   Extended length of HandleID

#### Return Value

True if the extended length of the specified center mark is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CenterMark::SetExtendedLength.

# ![](dotnetimages/collapse.gif)Example

[Extend Arms of Center Mark (VBA)](Extend_Arms_of_Center_Mark_Examples_VB.htm)

[Get and Set Center Mark Set (C#)](Get_and_Set_Center_Marks_Set_Example_CSharp.htm)

[Get and Set Center Mark Set (VB.NET)](Get_and_Set_Center_Marks_Set_Example_VBNET.htm)

[Get and Set Center Mark Set (VBA)](Get_and_Set_Center_Marks_Set_Example_VBA.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the center mark is in a center mark set (i.e., a linear or circular pattern), then use [ICenterMark::GroupCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark~GroupCount.html) to get the range of valid values for the GroupID parameter. You can use a value from 0 to ICenterMark::GroupCount for the GroupID parameter. To determine if a center mark is in a center mark set, use [ICenterMark::IsGrouped](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICenterMark~IsGrouped.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICenterMark Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark.html)

[ICenterMark Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark_members.html)

[ICenterMark::GetExtendedLength Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterMark~GetExtendedLength.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0