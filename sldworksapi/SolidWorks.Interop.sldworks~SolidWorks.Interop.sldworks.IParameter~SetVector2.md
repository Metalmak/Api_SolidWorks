<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~SetVector2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetVector2 Method (IParameter) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html) : SetVector2 Method (IParameter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   x value to store for the named configuration option

*Y*
:   y value to store for the named configuration option

*Z*
:   z value to store for the named configuration option

*ConfigurationOption*
:   Configuration option as defined in swInConfigurationOpts\_e

*ConfigurationName*
:   Name of the configuration

Sets the vector values of a named configuration option parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetVector2( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal ConfigurationOption As System.Integer, _    ByVal ConfigurationName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParameter Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim ConfigurationOption As System.Integer Dim ConfigurationName As System.String Dim value As System.Boolean   value = instance.SetVector2(X, Y, Z, ConfigurationOption, ConfigurationName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetVector2(     System.double X,    System.double Y,    System.double Z,    System.int ConfigurationOption,    System.string ConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetVector2(  &   System.double X, &   System.double Y, &   System.double Z, &   System.int ConfigurationOption, &   System.String^ ConfigurationName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   x value to store for the named configuration option

*Y*
:   y value to store for the named configuration option

*Z*
:   z value to store for the named configuration option

*ConfigurationOption*
:   Configuration option as defined in swInConfigurationOpts\_e

*ConfigurationName*
:   Name of the configuration

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Parameter::SetVector2.

# ![](dotnetimages/collapse.gif)Remarks

The ConfigurationName argument is:

* Not required if ConfigurationOption is set to swThisConfiguration = 1 or swAllConfiguration = 2.

  * Required if ConfigurationOption is set to swSpecifyConfiguration = 3.

Set the ConfigurationOption argument to swAllConfiguration = 2 for Drawing Docs as they do not have configurations.

# ![](dotnetimages/collapse.gif)See Also

####

[IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html)

[IParameter Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter_members.html)

[IParameter::GetVector Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~GetVector.html)

[IParameter::GetVectorVB Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~GetVectorVB.html)