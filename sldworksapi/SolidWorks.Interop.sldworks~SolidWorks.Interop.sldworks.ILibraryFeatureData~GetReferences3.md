<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~GetReferences3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetReferences3 Method (ILibraryFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILibraryFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData.html) : GetReferences3 Method (ILibraryFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Scope*
:   Reference scope as defined in swLibFeatureData\_e

*RefType*
:   Array of reference types as defined by swSelectType\_e

*RefName*
:   Array of reference names

Gets the references with respect to the specified scope.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetReferences3( _    ByVal Scope As System.Integer, _    ByRef RefType As System.Object, _    ByRef RefName As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILibraryFeatureData Dim Scope As System.Integer Dim RefType As System.Object Dim RefName As System.Object Dim value As System.Object   value = instance.GetReferences3(Scope, RefType, RefName) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetReferences3(     System.int Scope,    out System.object RefType,    out System.object RefName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetReferences3(  &   System.int Scope, &   [Out] System.Object^ RefType, &   [Out] System.Object^ RefName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Scope*
:   Reference scope as defined in swLibFeatureData\_e

*RefType*
:   Array of reference types as defined by swSelectType\_e

*RefName*
:   Array of reference names

#### Return Value

Array of references

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LibraryFeatureData::GetReferences3.

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

[ILibraryFeatureData::SetReferences Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~SetReferences.html)

[ILibraryFeatureData::ISetReferences Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~ISetReferences.html)

[ILibraryFeatureData::IGetReferences3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILibraryFeatureData~IGetReferences3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0