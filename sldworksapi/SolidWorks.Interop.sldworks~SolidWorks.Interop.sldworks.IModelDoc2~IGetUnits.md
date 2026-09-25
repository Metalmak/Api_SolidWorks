<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetUnits.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetUnits Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : IGetUnits Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the current unit settings, fraction base, fraction value, and significant digits.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetUnits() As System.Short ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim value As System.Short   value = instance.IGetUnits() ``` | |

| C# |  |
| --- | --- |
| ``` System.short IGetUnits() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.short IGetUnits(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

* in-process, unmanaged C++: Pointer to an array of 5 shorts (see **Remarks**)

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Units (C++)](Get_and_Set_Units_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

The format of the returned data is an array of shorts:

[ LengthUnit, FractionBase, FractionValue, SignificantDigits, RoundToFraction ]

where:

* LengthUnit =  current model units as defined in swLengthUnit\_e.

  * FractionBase =  decimal or fraction as defined in swFractionDisplay\_e; fractional units are only valid if the model units are set to swINCHES or swFEETINCHES.

    * FractionValue = denominator value if using fractional units.

      * SignificantDigits =  significant digits if using decimal units.

        * RoundToFraction =  flag denoting whether or not to round to the fraction; for example, if 4 was the denominator value and the actual value was .27, it is rounded to .25

You can also use [IModelDoc2::LengthUnit](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~LengthUnit.html), which provides access to the LengthUnit parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetAngularUnits.html)

[IModelDoc2::GetUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetUnits.html)

[IModelDoc2::IGetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetAngularUnits.html)

[IModelDoc2::IGetUserUnit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetUserUnit.html)

[IModelDoc2::GetUserUnit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetUserUnit.html)

[IModelDoc2::ISetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ISetAngularUnits.html)

[IModelDoc2::SetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetAngularUnits.html)

[IModelDoc2::SetUnits Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetUnits.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0