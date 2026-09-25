<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWLoadsAndRestraintsManager Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWLoadsAndRestraintsManager Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to managing [loads and restraints](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWLoadsAndRestraints.html).

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ICWLoadsAndRestraintsManager ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager ``` | |

| C# |  |
| --- | --- |
| ``` public interface ICWLoadsAndRestraintsManager ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ICWLoadsAndRestraintsManager ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager.

# ![](dotnetimages/collapse.gif)Example

[Analyze Part (C#)](Analyze_Part_Example_CSharp.htm)

[Analyze Part (VB.NET)](Analyze_Part_Example_VBNET.htm)

[Analyze Part (VBA)](Analyze_Part_Example_VB.htm)

[Create Linear Dynamic Study (VBA)](Create_Dynamic_Harmonic_Study_Example_VB.htm)

[Create Linear Dynamic Study (VB.NET)](Create_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Linear Dynamic Study (C#)](Create_Dynamic_Harmonic_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Define a different study for each set of loads and restraints that occur simultaneously.

* For structural studies (static, dynamic, buckling, frequency, and nonlinear), the following types are valid:

+ [Base excitation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBaseExcitation.html)

  + [Centrifugal force](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWCentriFugalForce.html)

    + [Distributed mass](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDistributedMass.html)

      + [Force](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWForce.html)

        + [Gravity](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWGravity.html)

          + [Pressure](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWPressure.html)

            + [Remote load](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad.html)

              + [Restraints](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRestraint.html) (specified displacements that can be zero or non-zero)

                + [Temperature](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWTemperature.html)

* For thermal studies, the following types are valid:

+ [Heat flux](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWHeatFlux.html)

  + [Convection](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWConvection.html)

    + [Radiation](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRadiation.html)

      + [Temperature](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWTemperature.html) (analogous to restraints for structural studies)

* For frequency studies, loads are not required but they are used if defined. If you solve frequency studies without specifying restraints, you will get six (6) additional rigid body modes.

# ![](dotnetimages/collapse.gif)Accessors

[ICWStudy::LoadsAndRestraintsManager](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudy~LoadsAndRestraintsManager.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWLoadsAndRestraints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraints.html)