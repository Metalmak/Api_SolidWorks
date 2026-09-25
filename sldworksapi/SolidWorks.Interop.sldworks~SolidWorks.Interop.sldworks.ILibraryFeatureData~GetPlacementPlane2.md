<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~GetPlacementPlane2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPlacementPlane2 Method (ILibraryFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILibraryFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData.html) : GetPlacementPlane2 Method (ILibraryFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Scope*
:   Placement scope as defined in swLibFeatureData\_e

*Type*
:   Placement type as defined in swSelectType\_e

Gets the face or plane on which the library feature was placed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlacementPlane2( _    ByVal Scope As System.Integer, _    ByRef Type As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILibraryFeatureData Dim Scope As System.Integer Dim Type As System.Integer Dim value As System.Object   value = instance.GetPlacementPlane2(Scope, Type) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetPlacementPlane2(     System.int Scope,    out System.int Type ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetPlacementPlane2(  &   System.int Scope, &   [Out] System.int Type ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Scope*
:   Placement scope as defined in swLibFeatureData\_e

*Type*
:   Placement type as defined in swSelectType\_e

#### Return Value

[Face](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) or [plane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LibraryFeatureData::GetPlacementPlane2.

# ![](dotnetimages/collapse.gif)Example

[Get Library Feature Data (VBA)](Get_Library_Feature_Data_Example_VB.htm)

[Get Library Feature Data (VB.NET)](Get_Library_Feature_Data_Example_VBNET.htm)

[Get Library Feature Data (C#)](Get_Library_Feature_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Accessing Selections that Define Features for additional details on using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[ILibraryFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData.html)

[ILibraryFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData_members.html)

[ILibraryFeatureData::SetPlacementPlane Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~SetPlacementPlane.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 SP1, Revision Number 18.1