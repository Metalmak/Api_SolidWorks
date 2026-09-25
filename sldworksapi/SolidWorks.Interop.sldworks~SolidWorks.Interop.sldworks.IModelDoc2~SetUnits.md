<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetUnits.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUnits Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetUnits Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UType*
:   Model units as defined in swLengthUnit\_e

*FractBase*
:   Decimal or fraction as defined in swFractionDisplay\_e

*FractDenom*
:   Denominator of the smallest inch fraction to be used, for example, 64 for 1/64; valid only if FractBase is set to swFRACTION (see **Remarks**)

*SigDigits*
:   Significant digits; valid only if FractBase is set to swDECIMAL

*RoundToFraction*
:   Flag denoting whether or not to round to the fraction; for example, if 4 is the denominator value given in FractDenom and the actual value is 0.27, it is rounded to 0.25

Sets the units used by the end-user for the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetUnits( _    ByVal UType As System.Short, _    ByVal FractBase As System.Short, _    ByVal FractDenom As System.Short, _    ByVal SigDigits As System.Short, _    ByVal RoundToFraction As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim UType As System.Short Dim FractBase As System.Short Dim FractDenom As System.Short Dim SigDigits As System.Short Dim RoundToFraction As System.Boolean   instance.SetUnits(UType, FractBase, FractDenom, SigDigits, RoundToFraction) ``` | |

| C# |  |
| --- | --- |
| ``` void SetUnits(     System.short UType,    System.short FractBase,    System.short FractDenom,    System.short SigDigits,    System.bool RoundToFraction ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetUnits(  &   System.short UType, &   System.short FractBase, &   System.short FractDenom, &   System.short SigDigits, &   System.bool RoundToFraction ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UType*
:   Model units as defined in swLengthUnit\_e

*FractBase*
:   Decimal or fraction as defined in swFractionDisplay\_e

*FractDenom*
:   Denominator of the smallest inch fraction to be used, for example, 64 for 1/64; valid only if FractBase is set to swFRACTION (see **Remarks**)

*SigDigits*
:   Significant digits; valid only if FractBase is set to swDECIMAL

*RoundToFraction*
:   Flag denoting whether or not to round to the fraction; for example, if 4 is the denominator value given in FractDenom and the actual value is 0.27, it is rounded to 0.25

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetUnits.

# ![](dotnetimages/collapse.gif)Example

' VBA
' 1. Open a document in SOLIDWORKS.
' 2. Run the macro below to set inch units with
'     a fractional base of 16 and no rounding.

Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Option Explicit
Sub main()
   Set swApp = Application.SldWorks
   Set Part = swApp.ActiveDoc
   Part.**SetUnits** swINCHES, swFRACTION, 16, 0, False
End Sub

# ![](dotnetimages/collapse.gif)Example

[Get and Set Units (C++)](Get_and_Set_Units_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

Fractional units are only valid if UType is set to swINCHES or swFEETINCHES.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetUnits.html)

[IModelDoc2::IGetUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetUnits.html)

[IModelDoc2::GetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetAngularUnits.html)

[IModelDoc2::GetUserUnit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetUserUnit.html)

[IModelDoc2::IGetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetAngularUnits.html)

[IModelDoc2::IGetUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetUnits.html)

[IModelDoc2::IGetUserUnit Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~IGetUserUnit.html)

[IModelDoc2::ISetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ISetAngularUnits.html)

[IModelDoc2::SetAngularUnits Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetAngularUnits.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0