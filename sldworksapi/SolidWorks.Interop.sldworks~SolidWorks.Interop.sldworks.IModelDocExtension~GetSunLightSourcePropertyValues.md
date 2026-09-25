<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSunLightSourcePropertyValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSunLightSourcePropertyValues Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetSunLightSourcePropertyValues Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NorthDirection*
:   [IMathVector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html); north direction of the sunlight source

*NorthLatitude*
:   North latitude of the sunlight source

*EastLongitude*
:   East longitude of the sunlight source

*TimeZone*
:   Standard time zone of the sunlight source

*DateTime*
:   Date and time stamp in the specified TimeZone

Gets the property values for a sunlight source.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSunLightSourcePropertyValues( _    ByRef NorthDirection As MathVector, _    ByRef NorthLatitude As System.Double, _    ByRef EastLongitude As System.Double, _    ByRef TimeZone As System.Double, _    ByRef DateTime As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim NorthDirection As MathVector Dim NorthLatitude As System.Double Dim EastLongitude As System.Double Dim TimeZone As System.Double Dim DateTime As System.String Dim value As System.Boolean   value = instance.GetSunLightSourcePropertyValues(NorthDirection, NorthLatitude, EastLongitude, TimeZone, DateTime) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetSunLightSourcePropertyValues(     out MathVector NorthDirection,    out System.double NorthLatitude,    out System.double EastLongitude,    out System.double TimeZone,    out System.string DateTime ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetSunLightSourcePropertyValues(  &   [Out] MathVector^ NorthDirection, &   [Out] System.double NorthLatitude, &   [Out] System.double EastLongitude, &   [Out] System.double TimeZone, &   [Out] System.String^ DateTime ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NorthDirection*
:   [IMathVector](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathVector.html); north direction of the sunlight source

*NorthLatitude*
:   North latitude of the sunlight source

*EastLongitude*
:   East longitude of the sunlight source

*TimeZone*
:   Standard time zone of the sunlight source

*DateTime*
:   Date and time stamp in the specified TimeZone

#### Return Value

True if getting the value is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetSunLightSourcePropertyValues.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Sunlight Source Property Values (VBA)](Get_and_Set_Sunlight_Source_Property_Values_Example_VB.htm)

[Get and Set Sunlight Source Property Values (VB.NET)](Get_and_Set_Sunlight_Source_Property_Values_Example_VBNET.htm)

[Get and Set Sunlight Source Property Values (C#)](Get_and_Set_Sunlight_Source_Property_Values_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::SetSunLightSourcePropertyValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetSunLightSourcePropertyValues.html)

[IModelDoc2::LightSourcePropertyValues Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~LightSourcePropertyValues.html)

[IModelDocExtension::GetSunLightAdvancedPropertyValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSunLightAdvancedPropertyValues.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0