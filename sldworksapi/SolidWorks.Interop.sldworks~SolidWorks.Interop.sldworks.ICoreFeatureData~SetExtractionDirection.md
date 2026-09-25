<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~SetExtractionDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetExtractionDirection Method (ICoreFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html) : SetExtractionDirection Method (ICoreFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PDir1*
:   Entity that defines the extraction direction (see **Remarks**)

*PDir2*
:   Entity that defines the extraction direction (see Remarks)

Sets the entities that define the extraction direction of this core feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetExtractionDirection( _    ByVal PDir1 As System.Object, _    ByVal PDir2 As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICoreFeatureData Dim PDir1 As System.Object Dim PDir2 As System.Object Dim value As System.Boolean   value = instance.SetExtractionDirection(PDir1, PDir2) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetExtractionDirection(     System.object PDir1,    System.object PDir2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetExtractionDirection(  &   System.Object^ PDir1, &   System.Object^ PDir2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PDir1*
:   Entity that defines the extraction direction (see **Remarks**)

*PDir2*
:   Entity that defines the extraction direction (see Remarks)

#### Return Value

True if the entities that define the extraction direction of this core feature are set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CoreFeatureData::SetExtractionDirection.

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

[ICoreFeatureData::GetExtractionDirection Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~GetExtractionDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0