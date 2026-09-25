<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetPrecision2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPrecision2 Method (IDisplayDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html) : SetPrecision2 Method (IDisplayDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Primary*
:   Number of digits displayed after the decimal point in the dimension value (see **Remarks**)

*Dual*
:   Number of digits displayed after the decimal point in the dual dimension value

*PrimaryTol*
:   Number of digits displayed after the decimal point in the tolerance value (see **Remarks**)

*DualTol*
:   Number of digits displayed after the decimal point in the dual tolerance value

Obsolete. Superseded by [IDisplayDimension::SetPrecision3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension~SetPrecision3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPrecision2( _    ByVal Primary As System.Integer, _    ByVal Dual As System.Integer, _    ByVal PrimaryTol As System.Integer, _    ByVal DualTol As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDisplayDimension Dim Primary As System.Integer Dim Dual As System.Integer Dim PrimaryTol As System.Integer Dim DualTol As System.Integer Dim value As System.Integer   value = instance.SetPrecision2(Primary, Dual, PrimaryTol, DualTol) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPrecision2(     System.int Primary,    System.int Dual,    System.int PrimaryTol,    System.int DualTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPrecision2(  &   System.int Primary, &   System.int Dual, &   System.int PrimaryTol, &   System.int DualTol ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Primary*
:   Number of digits displayed after the decimal point in the dimension value (see **Remarks**)

*Dual*
:   Number of digits displayed after the decimal point in the dual dimension value

*PrimaryTol*
:   Number of digits displayed after the decimal point in the tolerance value (see **Remarks**)

*DualTol*
:   Number of digits displayed after the decimal point in the dual tolerance value

#### Return Value

Return status (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DisplayDimension::SetPrecision2.

# ![](dotnetimages/collapse.gif)Remarks

The specified precision values must be in the range from 0 to 8, which indicates the number of digits after the decimal place to display that value. Alternatively, the precision values can be defined by swDimensionPrecisionSettings\_e.

| Parameter | swDimensionPrecisionSettings\_e value | Result |
| --- | --- | --- |
| * Primary* Dual* PrimaryTol* DualTol | swDoNotChangePrecisionSetting | The current setting is not changed. |
| * Primary* Dual* PrimaryTol* DualTol | swPrecisionFollowsDocumentSetting | The number of decimal places to display adheres to the document setting. Use [IModelDocExtension::GetUserPreferenceInteger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetUserPreferenceInteger.html)/ [IModelDocExtension::SetUserPreferenceInteger](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SetUserPreferenceInteger.html).swDetailingLinearDimPrecision, swDetailingAngularDimPrecision, or swDetailingAltLinearDimPrecision to get or set that value. |
| * PrimaryTol* DualTol | swTolerancePrecisionFollowsNominal | The number of decimal places to display is the same as for the dimension or dual dimension value. |

The return value indicates the success or failure of this method. In general, a value less than 0 indicates that the method failed and SOLIDWORKS did not set any precision values. A value of 0 indicates success. A value greater than 0 indicates that a problem occurred, but the method did not fail.

* -1  Method failed; no precision values were set.

  * 0   Method was successful; all precision values were set.

    * 1   Primary precision value was invalid.

      * 2   Alternate precision value was invalid.

        * 3   Primary tolerance precision value was invalid.

          * 4   Alternate tolerance precision value was invalid.

After using this method, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window to see your changes.

# ![](dotnetimages/collapse.gif)See Also

####

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDisplayDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0