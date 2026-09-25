<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~SetDoubleValue2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDoubleValue2 Method (IParameter) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html) : SetDoubleValue2 Method (IParameter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Value*
:   Value to store for the named configuration option

*ConfigurationOption*
:   Configuration option as defined in swSetValueInConfiguration\_e

*ConfigurationName*
:   Name of the configuration

Sets the double or integer value of a named configuration option parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDoubleValue2( _    ByVal Value As System.Double, _    ByVal ConfigurationOption As System.Integer, _    ByVal ConfigurationName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParameter Dim Value As System.Double Dim ConfigurationOption As System.Integer Dim ConfigurationName As System.String Dim value As System.Boolean   value = instance.SetDoubleValue2(Value, ConfigurationOption, ConfigurationName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDoubleValue2(     System.double Value,    System.int ConfigurationOption,    System.string ConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDoubleValue2(  &   System.double Value, &   System.int ConfigurationOption, &   System.String^ ConfigurationName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Value*
:   Value to store for the named configuration option

*ConfigurationOption*
:   Configuration option as defined in swSetValueInConfiguration\_e

*ConfigurationName*
:   Name of the configuration

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Parameter::SetDoubleValue2.

# ![](dotnetimages/collapse.gif)Example

[Create Attribute (VBA)](Create_Attribute_Example_VB.htm)

[Delete Attribute (C#)](Delete_Attribute_Example_CSharp.htm)

[Delete Attribute (VB.NET)](Delete_Attribute_Example_VBNET.htm)

[Delete Attribute (VBA)](Delete_Attribute_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The ConfigurationName argument is:

* Not required if ConfigurationOption is set to swSetValue\_InThisConfiguration = 1 or swSetValue\_InAllConfigurations = 2.

  * Required if ConfigurationOption is set to swSetValue\_InSpecificConfigurations = 3.

Set ConfigurationOption to swSetValue\_InAllConfigurations = 2 for drawing documents because they do not have configurations.

# ![](dotnetimages/collapse.gif)See Also

####

[IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html)

[IParameter Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter_members.html)

[IParameter::GetDoubleValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~GetDoubleValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0