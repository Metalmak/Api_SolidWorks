<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMassValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMassValues2 Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : GetMassValues2 Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   -1 or true to include mass in the remote load, 0 or false to not

Gets the components of mass in this remote load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMassValues2( _    ByRef BInclude As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Boolean Dim value As System.Object   value = instance.GetMassValues2(BInclude) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMassValues2(     out System.bool BInclude ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMassValues2(  &   [Out] System.bool BInclude ) ``` | |

#### Parameters

*BInclude*
:   -1 or true to include mass in the remote load, 0 or false to not

#### Return Value

Array of remote mass component values; valid only if BInclude = -1 (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

This method returns booleans or integers in out parameter BInclude, depending on its prior declaration.

If BInclude is cast as a:

* Boolean, true or false is returned in the out parameter.* Long or integer, -1 (=true) or 0 (=false) is returned in the out parameter.

This method is valid only if [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) = swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass.

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

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30