<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Add3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Add3 Method (IEquationMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html) : Add3 Method (IEquationMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   0-based index of the new equation (-1 places it at the end of the list)

*Equation*
:   String containing the equation (see **Remarks**)

*Solve*
:   True to solve the equation immediately; false to solve later (see **Remarks**)

*WhichConfigurations*
:   Configuration option as defined in swInConfigurationOpts\_e (see **Remarks**)

*ConfigNames*
:   Array of the names of the configurations to which to add this equation; valid only if WhichConfigurations is set to swInConfigurationOpts\_e.swSpecifyConfiguration, in which case, include the name of the current configuration in this array

Adds an equation at the specified index for the specified configurations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Add3( _    ByVal Index As System.Integer, _    ByVal Equation As System.String, _    ByVal Solve As System.Boolean, _    ByVal WhichConfigurations As System.Integer, _    ByVal ConfigNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEquationMgr Dim Index As System.Integer Dim Equation As System.String Dim Solve As System.Boolean Dim WhichConfigurations As System.Integer Dim ConfigNames As System.Object Dim value As System.Integer   value = instance.Add3(Index, Equation, Solve, WhichConfigurations, ConfigNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Add3(     System.int Index,    System.string Equation,    System.bool Solve,    System.int WhichConfigurations,    System.object ConfigNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Add3(  &   System.int Index, &   System.String^ Equation, &   System.bool Solve, &   System.int WhichConfigurations, &   System.Object^ ConfigNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   0-based index of the new equation (-1 places it at the end of the list)

*Equation*
:   String containing the equation (see **Remarks**)

*Solve*
:   True to solve the equation immediately; false to solve later (see **Remarks**)

*WhichConfigurations*
:   Configuration option as defined in swInConfigurationOpts\_e (see **Remarks**)

*ConfigNames*
:   Array of the names of the configurations to which to add this equation; valid only if WhichConfigurations is set to swInConfigurationOpts\_e.swSpecifyConfiguration, in which case, include the name of the current configuration in this array

#### Return Value

Index of the new equation if successfully added, -1 if error

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EquationMgr::Add3.

# ![](dotnetimages/collapse.gif)Example

[Add and Modify Equations (VBA)](Add_Equations_Example_VB.htm)

[Add and Modify Equations (VB.NET)](Add_Equations_Example_VBNET.htm)

[Add and Modify Equations (C#)](Add_Equations_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only works for parts having multiple configurations created in SOLIDWORKS 2014 or later. Use this method to add dimension equations, component equations, or global variable assignments to various configurations of models. If you don't have multiple configurations, then call [IEquationMgr::Add2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~Add2.html), which does not support configurations and is slightly faster.

To add an equation using the SOLIDWORKS user interface, you must embed the names of dimensions and global variables in double quotes:

* Global variable assignment:
  **"B" = 2**

  * Component equation:
    **"N\_SPOKES@CirPattern" = "BARLENGTH@Sketch2" /10**

    * Dimension equation that uses the Visual Basic IIf function:
      **"D1@Extrude2" = (IIf("D1@Extrude3">20, 15, 6))+5*** Dimension equation that sets a dimension to the current value:
        **"D1@Extrude2" =**

**NOTE:** To add an equation:

* you must specify Equation with the names of dimensions and global variables in double double quotes and the entire equation in double quotes. See the Examples.* directly to an assembly component's model, you must call [IAssemblyDoc::EditPart2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditPart2.html) before calling this method.

You can add a dimension equation whose left-hand side already exists, but only if the existing equation is suppressed. Adding the equation again unsuppresses it. See [IEquationMgr::ChangeSuppressionForAllConfigurations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~ChangeSuppressionForAllConfigurations.html) and [IEquationMgr::ChangeSuppressionForConfiguration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~ChangeSuppressionForConfiguration.html).

Setting Solve to false delays evaluation of this equation, which enhances performance when there are many equations to solve. When Solve is set to false, the equation appears in the FeatureManager design tree only after calling [IEquationMgr::EvaluateAll](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~EvaluateAll.html) or [IModelDoc2::EditRebuild3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html).

When adding global variable assignments and component equations, WhichConfigurations must be set to swInConfigurationOpts\_e.swAllConfiguration.

If you add a global variable assignment that already exists, this method returns an error.

To modify an equation added by this method, call [IEquationMgr::SetEquationAndConfigurationOption](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~SetEquationAndConfigurationOption.html).

When you add an equation, you are adding it to the list of relations. Thus, do not add an equation while traversing the equations in a model, because SOLIDWORKS could crash.

# ![](dotnetimages/collapse.gif)See Also

####

[IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html)

[IEquationMgr Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr_members.html)

[IEquationMgr::Delete Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Delete.html)

[IEquationMgr::GetCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetCount.html)

[IEquationMgr::Equation Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Equation.html)

[IEquationMgr::Status Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Status.html)

[IEquationMgr::GetConfigurationOption Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetConfigurationOption.html)

[IEquationMgr::IAdd3 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~IAdd3.html)

[IEquationMgr::ISetEquationAndConfigurationOption Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~ISetEquationAndConfigurationOption.html)

[IEquationMgr::Disabled Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Disabled.html)

[IEquationMgr::GetDisabledEquationCount Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetDisabledEquationCount.html)

[IEquationMgr::GlobalVariable Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GlobalVariable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0