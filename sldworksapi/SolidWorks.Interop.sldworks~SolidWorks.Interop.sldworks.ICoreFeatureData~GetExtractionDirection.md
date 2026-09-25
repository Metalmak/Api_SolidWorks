<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~GetExtractionDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetExtractionDirection Method (ICoreFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html) : GetExtractionDirection Method (ICoreFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type1*
:   Type of entity as defined in swSelectType\_e

*PDir1*
:   Entity that defines the extraction direction (see **Remarks**)

*Type2*
:   Type of entity as defined in swSelectType\_e

*PDir2*
:   Entity that defines the extraction direction (see Remarks)

Gets the entities that define the extraction direction of this core feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetExtractionDirection( _    ByRef Type1 As System.Integer, _    ByRef PDir1 As System.Object, _    ByRef Type2 As System.Integer, _    ByRef PDir2 As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICoreFeatureData Dim Type1 As System.Integer Dim PDir1 As System.Object Dim Type2 As System.Integer Dim PDir2 As System.Object Dim value As System.Integer   value = instance.GetExtractionDirection(Type1, PDir1, Type2, PDir2) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetExtractionDirection(     out System.int Type1,    out System.object PDir1,    out System.int Type2,    out System.object PDir2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetExtractionDirection(  &   [Out] System.int Type1, &   [Out] System.Object^ PDir1, &   [Out] System.int Type2, &   [Out] System.Object^ PDir2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type1*
:   Type of entity as defined in swSelectType\_e

*PDir1*
:   Entity that defines the extraction direction (see **Remarks**)

*Type2*
:   Type of entity as defined in swSelectType\_e

*PDir2*
:   Entity that defines the extraction direction (see Remarks)

#### Return Value

Number of entities that define the extraction direction

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CoreFeatureData::GetExtractionDirection.

# ![](dotnetimages/collapse.gif)Example

[Get Core Feature Data (C#)](Get_Core_Feature_Example_CSharp.htm)

[Get Core Feature Data (VB.NET)](Get_Core_Feature_Example_VBNET.htm)

[Get Core Feature Data (VBA)](Get_Core_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The types of entities that define the extraction direction are:

* Face

  * Plane

    * Edge

      * Vertex

        * Sketch line

          * Sketch point

There can be two entities because two sketch points can specify a direction.

# ![](dotnetimages/collapse.gif)See Also

####

[ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html)

[ICoreFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData_members.html)

[ICoreFeatureData::SetExtractionDirection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~SetExtractionDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0