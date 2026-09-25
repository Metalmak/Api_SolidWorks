<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~RevisionNumber.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RevisionNumber Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : RevisionNumber Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the version number of this SOLIDWORKS installation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RevisionNumber() As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim value As System.String   value = instance.RevisionNumber() ``` | |

| C# |  |
| --- | --- |
| ``` System.string RevisionNumber() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ RevisionNumber(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

SOLIDWORKS version number (See **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::RevisionNumber.

# ![](dotnetimages/collapse.gif)Example

[Create Infinite Plane (VBA)](Create_Infinite_Plane_Example_VB.htm)

[Get Material Property Names (VBA)](Get_Material_Property_Names_Example_VB.htm)

[Get Version Number (C#)](Get_Version_Number_Example_CSharp.htm)

[Get Version Number (VB.NET)](Get_Version_Number_Example_VBNET.htm)

[Get Version Number (VBA)](Get_Version_Number_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns a string in the form "*major*.*minor*", where *major* is an integer (e.g., 1), and *minor* is a decimal number (e.g., 0.0).

For all SOLIDWORKS executables prior to the initial public release of SOLIDWORKS 2000, this method returns 1.0.0 (major = 1, minor = 0.0).

For the initial public release of SOLIDWORKS 2000, this method returns 8.0.0 (major = 8, minor = 0.0). For SOLIDWORKS 2000 SP1, this method returns 8.1.0, and each successive service pack or service pack hot fix of SOLIDWORKS 2000 increments the minor decimal number (e.g., SP1.1 returns **8.1.1**, SP2 returns **8.2.0**, SP3 returns **8.3.0**, etc.).

For the inital public release of SOLIDWORKS 2005, this method returns 13.0.0. For SOLIDWORKS 2005 SP0.1, it returns 13.0.1. For SOLIDWORKS 2005 SP1, it returns 13.1.0.

In general, each successive major public release increments the major number by one, each service pack increments the minor decimal number by 1.0, and each service pack hot fix increments the minor decimal number by 0.1. For the initial public release, the minor decimal number is always 0.0.

Alpha, beta, and pre-release versions return negative minor decimal numbers:

* a1:    **-1.0*** b1:    **-2.0*** b2:   **-3.0*** b3:    **-4.0*** PR1:  **-5.0** (This value might be lower or higher depending on the number of beta releases.)

For SOLIDWORKS 2015 b2, this method returns **23.-3.0**.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::VersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~VersionHistory.html)

[ISldWorks::IVersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~IVersionHistory.html)

[IModelDoc2::VersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~VersionHistory.html)

[IModelDoc2::IVersionHistory Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IVersionHistory.html)

[ISldWorks::GetBuildNumbers2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetBuildNumbers2.html)

Accessing SOLIDWORKS Add-in Objects