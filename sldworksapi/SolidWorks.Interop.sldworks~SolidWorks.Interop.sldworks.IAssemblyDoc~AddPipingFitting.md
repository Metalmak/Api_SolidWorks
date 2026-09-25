<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddPipingFitting.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddPipingFitting Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddPipingFitting Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PathName*
:   Full name and directory location of part file used for this fitting

*ConfigName*
:   Configuration within the fitting part file which should be used

*AlignmentIndex*
:   Each fitting has a varying number of alignment positions; this value allows you to choose the alignment position

Adds a pipe fitting to the current piping assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddPipingFitting( _    ByVal PathName As System.String, _    ByVal ConfigName As System.String, _    ByVal AlignmentIndex As System.Short _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim PathName As System.String Dim ConfigName As System.String Dim AlignmentIndex As System.Short Dim value As System.Boolean   value = instance.AddPipingFitting(PathName, ConfigName, AlignmentIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddPipingFitting(     System.string PathName,    System.string ConfigName,    System.short AlignmentIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddPipingFitting(  &   System.String^ PathName, &   System.String^ ConfigName, &   System.short AlignmentIndex ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PathName*
:   Full name and directory location of part file used for this fitting

*ConfigName*
:   Configuration within the fitting part file which should be used

*AlignmentIndex*
:   Each fitting has a varying number of alignment positions; this value allows you to choose the alignment position

#### Return Value

True if successful, false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddPipingFitting.

# ![](dotnetimages/collapse.gif)Remarks

This method adds a piping fitting to the selected sketch point. The sketch must be the active sketch of the piping assembly.

The alignmentIndex argument controls the alignment of the fitting. For example, you can align a t-piece in two ways: passing 0 aligns the t-piece one way, and passing 1 aligns it the other way.

If the routing DLL is not available, then COM returns ITF\_E\_ROUTINGNOTLOADED.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddPipePenetration Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddPipePenetration.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207