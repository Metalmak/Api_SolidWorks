<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceEndEdit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ForceEndEdit Method (ICWForce) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : ForceEndEdit Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Ends editing a force.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ForceEndEdit() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim value As System.Integer   value = instance.ForceEndEdit() ``` | |

| C# |  |
| --- | --- |
| ``` System.int ForceEndEdit() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ForceEndEdit(); ``` | |

#### Return Value

Error as defined in [swsForceEndEditError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceEndEditError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::ForceEndEdit.

# ![](dotnetimages/collapse.gif)Example

[Add Nonuniform Force Distribution (VBA)](Add_Force_Example_VB.htm)

[Add Nonuniform Force Distribution (VB.NET)](Add_Force_Example_VBNET.htm)

[Add Nonuniform Force Distribution (C#)](Add_Force_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You must call [ICWForce::ForceBeginEdit](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWForce~ForceBeginEdit.html) to start editing this force. To end editing this force, you must call this method. Changes are not applied unless you call both methods.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0