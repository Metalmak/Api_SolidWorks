<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ImportDiagnosis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ImportDiagnosis Method (IPartDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : ImportDiagnosis Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CloseAllGaps*
:   True to repair any gaps, false to not

*RemoveFaces*
:   True to remove any bad faces and create gaps in the feature, false to not

*FixFaces*
:   True to fix the bad faces, false to not

*Options*
:   Not used

Diagnoses and repairs any gaps or bad faces on imported features.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ImportDiagnosis( _    ByVal CloseAllGaps As System.Boolean, _    ByVal RemoveFaces As System.Boolean, _    ByVal FixFaces As System.Boolean, _    ByVal Options As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim CloseAllGaps As System.Boolean Dim RemoveFaces As System.Boolean Dim FixFaces As System.Boolean Dim Options As System.Integer Dim value As System.Integer   value = instance.ImportDiagnosis(CloseAllGaps, RemoveFaces, FixFaces, Options) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ImportDiagnosis(     System.bool CloseAllGaps,    System.bool RemoveFaces,    System.bool FixFaces,    System.int Options ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ImportDiagnosis(  &   System.bool CloseAllGaps, &   System.bool RemoveFaces, &   System.bool FixFaces, &   System.int Options ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CloseAllGaps*
:   True to repair any gaps, false to not

*RemoveFaces*
:   True to remove any bad faces and create gaps in the feature, false to not

*FixFaces*
:   True to fix the bad faces, false to not

*Options*
:   Not used

#### Return Value

>= 0 if import diagnosis is successful, -1 if an error occurred

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::ImportDiagnosis.

# ![](dotnetimages/collapse.gif)Example

[Import STEP File (C#)](Import_STEP_File_Example_CSharp.htm)

[Import STEP File (VB.NET)](Import_STEP_File_Example_VBNET.htm)

[Import STEP File (VBA)](Import_STEP_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use this method for an imported solid body that has rebuild errors or for an imported surface that did not knit into a solid body.

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IPartDoc::ImportDiagnosisGapCloser Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~ImportDiagnosisGapCloser.html)

[IBody2::Diagnose Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Diagnose.html)

[IDiagnoseResult Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDiagnoseResult.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207