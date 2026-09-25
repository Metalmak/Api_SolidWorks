<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~ISetEquationAndConfigurationOption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISetEquationAndConfigurationOption Method (IEquationMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html) : ISetEquationAndConfigurationOption Method (IEquationMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index of the equation to modify

*Equation*
:   String containing the modified equation (see **Remarks**)

*WhichConfigurations*
:   Configuration option as defined in swInConfigurationOpts\_e

*ConfigCount*
:   Number of names in ConfigNames array

*ConfigNames*
:   * in-process, in-process, unmanaged C++: Pointer to an array of strings containing configuration names

    * VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Modifies the equation at the specified index for the specified configurations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ISetEquationAndConfigurationOption( _    ByVal Index As System.Integer, _    ByVal Equation As System.String, _    ByVal WhichConfigurations As System.Integer, _    ByVal ConfigCount As System.Integer, _    ByRef ConfigNames As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEquationMgr Dim Index As System.Integer Dim Equation As System.String Dim WhichConfigurations As System.Integer Dim ConfigCount As System.Integer Dim ConfigNames As System.String Dim value As System.Integer   value = instance.ISetEquationAndConfigurationOption(Index, Equation, WhichConfigurations, ConfigCount, ConfigNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ISetEquationAndConfigurationOption(     System.int Index,    System.string Equation,    System.int WhichConfigurations,    System.int ConfigCount,    ref System.string ConfigNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ISetEquationAndConfigurationOption(  &   System.int Index, &   System.String^ Equation, &   System.int WhichConfigurations, &   System.int ConfigCount, &   System.String^% ConfigNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index of the equation to modify

*Equation*
:   String containing the modified equation (see **Remarks**)

*WhichConfigurations*
:   Configuration option as defined in swInConfigurationOpts\_e

*ConfigCount*
:   Number of names in ConfigNames array

*ConfigNames*
:   * in-process, in-process, unmanaged C++: Pointer to an array of strings containing configuration names

    * VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

#### Return Value

0 if equation successfully added, -1 if error

# ![](dotnetimages/collapse.gif)Remarks

This method modifies only equations added using [IEquationMgr::IAdd3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~IAdd3.html).

To add an equation using the SOLIDWORKS user interface, you must embed the names of dimensions and global variables in double quotes:

* Global variable assignment:
  **"B" = 2**

  * Component equation:
    **"N\_SPOKES@CirPattern" = "BARLENGTH@Sketch2" /10**

    * Dimension equation that uses the Visual Basic IIf function:
      **"D1@Extrude2" = (IIf("D1@Extrude3">20, 15, 6))+5*** Dimension equation that sets a dimension to the current value:
        **"D1@Extrude2" =*** Dimension equation that modifies the right-hand side of an already existing dimension equation:
          **"D1@Extrude2" = 0.05**

**NOTES:**

* To modify an equation:

  + you must specify Equation with the names of dimensions and global variables in double double quotes and the entire equation in double quotes. The examples for [IEquationMgr::Add3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~Add3.html) show how to do this. [Global variables](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GlobalVariable.html) cannot be set to current values using this method.+ added directly to an assembly component's model, you must call [IAssemblyDoc::EditPart2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditPart2.html) before calling this method.

  * If you change the active configuration, then you must call [IModelDoc2::GetEquationMgr](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetEquationMgr.html) again.* If the model has just one configuration, then use [IEquationMgr::Equation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Equation.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html)

[IEquationMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr_members.html)

[IEquationMgr::SetEquationAndConfigurationOption Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~SetEquationAndConfigurationOption.html)

[IEquationMgr::GetConfigurationOption Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetConfigurationOption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0