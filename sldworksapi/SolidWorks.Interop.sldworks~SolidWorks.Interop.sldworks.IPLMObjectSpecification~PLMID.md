<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPLMObjectSpecification~PLMID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PLMID Property (IPLMObjectSpecification) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPLMObjectSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPLMObjectSpecification.html) : PLMID Property (IPLMObjectSpecification) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the ID of a SOLIDWORKS Connected document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property PLMID As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPLMObjectSpecification Dim value As System.String   instance.PLMID = value   value = instance.PLMID ``` | |

| C# |  |
| --- | --- |
| ``` System.string PLMID {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ PLMID {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Document ID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PLMObjectSpecification::PLMID.

# ![](dotnetimages/collapse.gif)Example

See the [IPLMObjectSpecification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPLMObjectSpecification.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IPLMObjectSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPLMObjectSpecification.html)

[IPLMObjectSpecification Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPLMObjectSpecification_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 SP3.1, Revision Number 28.3.1