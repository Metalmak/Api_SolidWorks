<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~Equation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| Equation Property (ICWPressure) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html) : Equation Property (ICWPressure) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the equation describing this pressure of nonuniform distribution.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Equation As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWPressure Dim value As System.String   instance.Equation = value   value = instance.Equation ``` | |

| C# |  |
| --- | --- |
| ``` System.string Equation {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ Equation {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

#### Property Value

Nonuniform pressure distribution equation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWPressure::Equation.

# ![](dotnetimages/collapse.gif)Example

```
For VBA:
```

```
CWPressureObj.CoordSystemType = swsCoordinateTypeCylindrical

CWPressureObj.Equation = ".4*""r"" +.8* ""t"" +.6* ""z"""
```

```
For VB.NET:
```

```
CWPressureObj.CoordSystemType = swsCoordinateType_e.swsCoordinateTypeCylindrical

CWPressureObj.Equation = ".4*""r"" +.8* ""t"" +.6* ""z"""
```

```
For C#:
```

```
CWPressureObj.CoordSystemType = (int)swsCoordinateType_e.swsCoordinateTypeCylindrical;

CWPressureObj.Equation = ".4*\"r\" +.8* \"t\" +.6* \"z\"";
```

```
See the ICWPressure examples.
```

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWPressure::IncludeNonUniformDistribution](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~IncludeNonUniformDistribution.html) is set to 1.

The equation is a string that contains double-quoted coordinate variables. In the example, the cylindrical coordinate system requires that the equation be specified with coordinate variables r, t, and z. Other coordinate systems use different sets of coordinate variables. See the **Defining Nonuniform Pressure Loads** topic in the SOLIDWORKS Simulation Help for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWPressure Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure.html)

[ICWPressure Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure_members.html)

[ICWPressure::CoordSystemType Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~CoordSystemType.html)

[ICWPressure::EquationAngularUnit Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationAngularUnit.html)

[ICWPressure::EquationLinearUnit Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~EquationLinearUnit.html)

[ICWPressure::GetCoordinateSystem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~GetCoordinateSystem.html)

[ICWPressure::SetCoordinateSystem Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWPressure~SetCoordinateSystem.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0