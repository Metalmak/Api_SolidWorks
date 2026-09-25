<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMassValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMassValues Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetMassValues Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   1 to include mass in the remote load, 0 to not

*Var*
:   Array of mass component values for this remote load; valid only if BInclude = 1 (see **Remarks**)

Obsolete. Superseded by [ICWRemoteLoad::SetMassValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMassValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMassValues( _    ByVal BInclude As System.Integer, _    ByVal Var As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Integer Dim Var As System.Object   instance.SetMassValues(BInclude, Var) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMassValues(     System.int BInclude,    System.object Var ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMassValues(  &   System.int BInclude, &   System.Object^ Var ) ``` | |

#### Parameters

*BInclude*
:   1 to include mass in the remote load, 0 to not

*Var*
:   Array of mass component values for this remote load; valid only if BInclude = 1 (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::SetMassValues.

# ![](dotnetimages/collapse.gif)Remarks

This method works only if [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) = swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass.

Array of mass components:

> **[** m*, Lxx, Lyy, Lzz, Lxy, Lyz, Lxz* **]**

where:

* m = Remote mass value

  * Lxx = Mass moment of inertia with respect to axis X

    * Lyy = Mass moment of inertia with respect to axis Y

      * Lzz = Mass moment of inertia with respect to axis Z

        * Lxy = Product of inertias with respect to axes X and Y

          * Lyz = Product of inertias with respect to axes Y and Z

            * Lxz = Product of inertias with respect to axes X and Z

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

[ICWRemoteLoad::GetMassValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMassValues.html)

[ICWRemoteLoad::MassUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~MassUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0