<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertJoin2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertJoin2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : InsertJoin2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*HideParts*
:   True hides the original components after the join is complete, false shows them

*ForceContact*
:   True joins any coincident faces and intruding volumes, false does not

Constructs a feature from merged selected components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertJoin2( _    ByVal HideParts As System.Boolean, _    ByVal ForceContact As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim HideParts As System.Boolean Dim ForceContact As System.Boolean Dim value As System.Boolean   value = instance.InsertJoin2(HideParts, ForceContact) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool InsertJoin2(     System.bool HideParts,    System.bool ForceContact ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool InsertJoin2(  &   System.bool HideParts, &   System.bool ForceContact ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*HideParts*
:   True hides the original components after the join is complete, false shows them

*ForceContact*
:   True joins any coincident faces and intruding volumes, false does not

#### Return Value

True if feature creation was successful, false if it was not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::InsertJoin2.

# ![](dotnetimages/collapse.gif)Example

[Insert Join Feature (C#)](Insert_Join_Feature_Example_CSharp.htm)

[Insert Join Feature (VB.NET)](Insert_Join_Feature_Example_VBNET.htm)

[Insert Join Feature (VBA)](Insert_Join_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

When you use this method, SOLIDWORKS must be in Edit Part mode for the target part. You must also preselect the component parts to be merged into the edited part.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IJoinFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IJoinFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0