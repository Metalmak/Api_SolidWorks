<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~IncludeTypeWithKey.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IncludeTypeWithKey Property (ICWPinConnector) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPinConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector.html) : IncludeTypeWithKey Property (ICWPinConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to prevent relative rotation between the two cylindrical faces of this pin connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IncludeTypeWithKey As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPinConnector Dim value As System.Boolean   instance.IncludeTypeWithKey = value   value = instance.IncludeTypeWithKey ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IncludeTypeWithKey {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IncludeTypeWithKey {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True to prevent relative rotation between the two cylindrical faces, false to not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPinConnector::IncludeTypeWithKey.

# ![](dotnetimages/collapse.gif)Example

[Create and Edit Bolt and Pin Connectors (VBA)](Create_and_Edit_Bolt_and_Pin_Connectors_Example_VB.htm)

[Create and Edit Bolt and Pin Connectors (VB.NET)](Create_and_Edit_Bolt_and_Pin_Connectors_Example_VBNET.htm)

[Create and Edit Bolt and Pin Connectors (C#)](Create_and_Edit_Bolt_and_Pin_Connectors_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If this property is set to true, then:

* Do not set [ICWPinConnector::RotationalStiffnessValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~RotationalStiffnessValue.html).* Do set [ICWPinConnector::AxialStiffnessValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~AxialStiffnessValue.html) only if [ICWPinConnector::IncludeTypeWithRetainerRing](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector~IncludeTypeWithRetainerRing.html) is set to false.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPinConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector.html)

[ICWPinConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPinConnector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0