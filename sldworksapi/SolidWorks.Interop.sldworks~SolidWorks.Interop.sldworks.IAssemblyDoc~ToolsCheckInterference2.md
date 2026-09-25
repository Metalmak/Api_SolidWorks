<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ToolsCheckInterference2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ToolsCheckInterference2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : ToolsCheckInterference2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumComponents*
:   Number of components to check

*LpComponents*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) being checked for interference

*CoincidentInterference*
:   True to treat coincident entities as interference, false to not

*PComp*
:   Array of components where interferences have been found

*PFace*
:   Array of [faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) where interferences have been found

Checks for interference between parts in this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ToolsCheckInterference2( _    ByVal NumComponents As System.Integer, _    ByVal LpComponents As System.Object, _    ByVal CoincidentInterference As System.Boolean, _    ByRef PComp As System.Object, _    ByRef PFace As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim NumComponents As System.Integer Dim LpComponents As System.Object Dim CoincidentInterference As System.Boolean Dim PComp As System.Object Dim PFace As System.Object   instance.ToolsCheckInterference2(NumComponents, LpComponents, CoincidentInterference, PComp, PFace) ``` | |

| C# |  |
| --- | --- |
| ``` void ToolsCheckInterference2(     System.int NumComponents,    System.object LpComponents,    System.bool CoincidentInterference,    out System.object PComp,    out System.object PFace ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ToolsCheckInterference2(  &   System.int NumComponents, &   System.Object^ LpComponents, &   System.bool CoincidentInterference, &   [Out] System.Object^ PComp, &   [Out] System.Object^ PFace ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumComponents*
:   Number of components to check

*LpComponents*
:   Array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) being checked for interference

*CoincidentInterference*
:   True to treat coincident entities as interference, false to not

*PComp*
:   Array of components where interferences have been found

*PFace*
:   Array of [faces](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) where interferences have been found

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::ToolsCheckInterference2.

# ![](dotnetimages/collapse.gif)Example

[Check Interference (VBA)](Check_Interference_using_AssemblyDoc_ToolsCheckInterference2_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns:

* an empty array of faces for components that have coincident faces that touch.

  * an array of components for components that touch.

For each face that intersects, there is a corresponding component.

**NOTE:** The obsolete method, IAssemblyDoc::ToolsCheckInterference, displays the Interference Detection PropertyManager, but this method does not.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::IToolsCheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IToolsCheckInterference3.html)

[IInterferenceDetectionMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterferenceDetectionMgr.html)

[IInterference Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IInterference.html)

[IModeler::ICheckInterferenceCount3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterferenceCount3.html)

[IModeler::ICheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterference3.html)

[IModeler::CheckInterference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~CheckInterference3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0