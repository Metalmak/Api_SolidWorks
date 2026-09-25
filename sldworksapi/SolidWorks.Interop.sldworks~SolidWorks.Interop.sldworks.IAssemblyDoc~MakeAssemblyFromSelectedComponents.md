<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~MakeAssemblyFromSelectedComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MakeAssemblyFromSelectedComponents Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : MakeAssemblyFromSelectedComponents Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Path and filename of the new assembly

Creates a new assembly comprised of the selected components of this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function MakeAssemblyFromSelectedComponents( _    ByVal FileName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim FileName As System.String Dim value As System.Boolean   value = instance.MakeAssemblyFromSelectedComponents(FileName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool MakeAssemblyFromSelectedComponents(     System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool MakeAssemblyFromSelectedComponents(  &   System.String^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Path and filename of the new assembly

#### Return Value

True if a new assembly is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::MakeAssemblyFromSelectedComponents.

# ![](dotnetimages/collapse.gif)Example

[Make Assembly From Selected Components (VB.NET)](Make_Assembly_From_Selected_Components_Example_VBNET.htm)

[Make Assembly From Selected Components (VBA)](Make_Assembly_From_Selected_Components_Example_VB.htm)

[Make Assembly From Selected Components (C#)](Make_Assembly_From_Selected_Components_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If **Tools > Options > System Options > Assemblies >  Save new components to external files** is selected, then a virtual sub-assembly is created and saved to an external file. Be sure to save the parent assembly before calling this method.

If **Tools > Options > System Options > Assemblies >  Save new components to external files** is not selected, then the *FileName* input parameter is ignored, and only a virtual sub-assembly is created.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0