<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~SetStringValue2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetStringValue2 Method (IParameter) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html) : SetStringValue2 Method (IParameter) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StringValue*
:   Value to store for the named configuration option

*ConfigurationOption*
:   Configuration option as defined in swInConfigurationOpts\_e

*ConfigurationName*
:   Name of the configuration

Sets the double or integer value of a named configuration option parameter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetStringValue2( _    ByVal StringValue As System.String, _    ByVal ConfigurationOption As System.Integer, _    ByVal ConfigurationName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParameter Dim StringValue As System.String Dim ConfigurationOption As System.Integer Dim ConfigurationName As System.String Dim value As System.Boolean   value = instance.SetStringValue2(StringValue, ConfigurationOption, ConfigurationName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetStringValue2(     System.string StringValue,    System.int ConfigurationOption,    System.string ConfigurationName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetStringValue2(  &   System.String^ StringValue, &   System.int ConfigurationOption, &   System.String^ ConfigurationName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StringValue*
:   Value to store for the named configuration option

*ConfigurationOption*
:   Configuration option as defined in swInConfigurationOpts\_e

*ConfigurationName*
:   Name of the configuration

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Parameter::SetStringValue2.

# ![](dotnetimages/collapse.gif)Example

[Create Attribute (VBA)](Create_Attribute_Example_VB.htm)

[Delete Attribute (C#)](Delete_Attribute_Example_CSharp.htm)

[Delete Attribute (VB.NET)](Delete_Attribute_Example_VBNET.htm)

[Delete Attribute (VBA)](Delete_Attribute_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The ConfigurationName argument is:

* Not required if ConfigurationOption is set to swThisConfiguration = 1 or swAllConfiguration = 2.

  * Required if ConfigurationOption is set to swSpecifyConfiguration =3 .

Set ConfigurationOption to swAllConfiguration = 2 for drawing documents because they do not have configurations.

# ![](dotnetimages/collapse.gif)See Also

####

[IParameter Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter.html)

[IParameter Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter_members.html)

[IParameter::GetStringValue Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParameter~GetStringValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001 FCS, Revision Number 9.0