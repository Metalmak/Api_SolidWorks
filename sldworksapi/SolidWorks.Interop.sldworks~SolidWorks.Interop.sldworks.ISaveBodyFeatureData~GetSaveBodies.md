<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData~GetSaveBodies.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSaveBodies Method (ISaveBodyFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISaveBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData.html) : GetSaveBodies Method (ISaveBodyFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Bodies*
:   :   Array of save bodies

*FilePaths*
:   Array of paths and filenames for the part documents of Bodies

*Flags*
:   :   Array of booleans indicating whether each corresponding save body is consumed; true if removed from the original part, false if not

Gets the save bodies in this Save Bodies feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetSaveBodies( _    ByRef Bodies As System.Object, _    ByRef FilePaths As System.Object, _    ByRef Flags As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISaveBodyFeatureData Dim Bodies As System.Object Dim FilePaths As System.Object Dim Flags As System.Object   instance.GetSaveBodies(Bodies, FilePaths, Flags) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSaveBodies(     out System.object Bodies,    out System.object FilePaths,    out System.object Flags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSaveBodies(  &   [Out] System.Object^ Bodies, &   [Out] System.Object^ FilePaths, &   [Out] System.Object^ Flags ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Bodies*
:   :   Array of save bodies

*FilePaths*
:   Array of paths and filenames for the part documents of Bodies

*Flags*
:   :   Array of booleans indicating whether each corresponding save body is consumed; true if removed from the original part, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SaveBodyFeatureData::GetSaveBodies.

# ![](dotnetimages/collapse.gif)Remarks

See Accessing Selections that Define Features for additional details on using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISaveBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData.html)

[ISaveBodyFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData_members.html)

[ISaveBodyFeatureData::GetSaveBodiesCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData~GetSaveBodiesCount.html)

[ISaveBodyFeatureData::AddSaveBodies Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData~AddSaveBodies.html)

[ISaveBodyFeatureData::RemoveSaveBodies Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISaveBodyFeatureData~RemoveSaveBodies.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0