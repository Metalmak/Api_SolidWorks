<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStraightTapElementData~Equation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Equation Property (IStraightTapElementData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IStraightTapElementData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStraightTapElementData.html) : Equation Property (IStraightTapElementData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the equation for the blind depth or offset distance of this straight tap hole element.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Equation As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IStraightTapElementData Dim value As System.Integer   instance.Equation = value   value = instance.Equation ``` | |

| C# |  |
| --- | --- |
| ``` System.int Equation {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int Equation {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Equation for the blind depth or offset distance as defined in swStraightTapHoleEquation\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See StraightTapElementData::Equation.

# ![](dotnetimages/collapse.gif)Remarks

If [IAdvancedHoleFeatureData::UseBaselineDimensions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleFeatureData~UseBaselineDimensions.html) is set to false, and:

* [IAdvancedHoleElementData::EndCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData~EndCondition.html) is set to swEndConditions\_e.swEndCondBlind, then this property specifies the equation for the depth of the Blind end condition. If this property is set to swStraightTapeHoleEquation\_e.swStraightTapHoleEquation\_UserDefinedValue, then use [IAdvancedHoleElementData::BlindDepth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData~BlindDepth.html) to set the custom Blind depth of this hole element.* IAdvancedHoleElementData::EndCondition is specifically set to anything other than Blind, then this property is not valid.

If IAdvancedHoleFeatureData::UseBaselineDimensions is set to true, then:

* the end condition automatically becomes swEndConditions\_e.swEndCondOffsetFromSurface,

   - and -

* this property specifies the equation for the offset distance. If this property is set to swStraightTapHoleEquation\_e.swStraightTapHoleEquation\_UserDefinedValue, then use [IAdvancedHoleElementData::OffsetDistance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedHoleElementData~OffsetDistance.html) to set the custom offset distance of this hole element.

# ![](dotnetimages/collapse.gif)See Also

####

[IStraightTapElementData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStraightTapElementData.html)

[IStraightTapElementData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IStraightTapElementData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0