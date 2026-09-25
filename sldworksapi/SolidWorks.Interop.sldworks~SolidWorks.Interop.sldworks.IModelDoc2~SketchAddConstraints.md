<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchAddConstraints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchAddConstraints Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchAddConstraints Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IdStr*
:   Constraint (see **Remarks**)

Adds the specified constraint to the selected entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchAddConstraints( _    ByVal IdStr As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim IdStr As System.String   instance.SketchAddConstraints(IdStr) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchAddConstraints(     System.string IdStr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchAddConstraints(  &   System.String^ IdStr ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IdStr*
:   Constraint (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchAddConstraints.

# ![](dotnetimages/collapse.gif)Example

[Constrain Sketch (VBA)](Constrain_Sketch_Example_VB.htm)

[Constrain Sketch (VB.NET)](Constrain_Sketch_Example_VBNET.htm)

[Constrain Sketch (C#)](Constrain_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **SOLIDWORKS 2005 and earlier** | **SOLIDWORKS 2006 and later** |
| * sgHORIZONTAL (2D sketch) * sgHORIZONTAL (3D sketch) * sgHORIZPOINTS (2D sketch) * sgHORIZPOINTS (3D sketch) * sgVERTICAL (2D sketch) * sgVERTICAL (3D sketch) * sgVERTPOINTS (2D sketch) * sgVERTPOINTS (3D sketch) * sgALONGZPOINTS * sgALONGZ * sgCOLINEAR * sgCORADIAL * sgPERPENDICULAR * sgPARALLEL * sgTANGENT * sgCONCENTRIC * sgCOINCIDENT * sgSYMMETRIC * sgATMIDDLE * sgATINTERSECT * sgATPIERCE * sgFIXED * sgANGLE * sgARCANG180 * sgARCANG270 * sgARCANG90 * sgARCANGBOTTOM * sgARCANGLEFT * sgARCANGRIGHT * sgARCANGTOP * sgDIAMETER * sgDISTANCE * sgSAMELENGTH * sgOFFSETEDGE * sgSNAPANGLE * sgSNAPGRID * sgSNAPLENGTH * sgUSEEDGE | * sgHORIZONTAL2D * sgALONGX3D * sgHORIZONTALPOINTS2D * sgALONGXPOINTS3D * sgVERTICAL2D * sgALONGY3D * sgVERTPOINTS2D * sgALONGYPOINTS3D * sgALONGZPOINTS3D * sgALONGZ3D * sgCOLINEAR * sgCORADIAL * sgPERPENDICULAR * sgPARALLEL * sgTANGENT * sgCONCENTRIC * sgCOINCIDENT * sgSYMMETRIC * sgATMIDDLE * sgATINTERSECT * sgATPIERCE * sgFIXED * sgANGLE * sgARCANG180 * sgARCANG270 * sgARCANG90 * sgARCANGBOTTOM * sgARCANGLEFT * sgARCANGRIGHT * sgARCANGTOP * sgDIAMETER * sgDISTANCE * sgSAMELENGTH * sgOFFSETEDGE * sgSNAPANGLE * sgSNAPGRID * sgSNAPLENGTH * sgUSEEDGE * sgMERGEPOINTS |

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::SketchConstrainCoincident Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstrainCoincident.html)

[IModelDoc2::SketchConstrainConcentric Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstrainConcentric.html)

[IModelDoc2::SketchConstrainParallel Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstrainParallel.html)

[IModelDoc2::SketchConstrainPerp Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstrainPerp.html)

[IModelDoc2::SketchConstrainTangent Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstrainTangent.html)

[IModelDoc2::SketchConstraintsDel Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstraintsDel.html)

[IModelDoc2::SketchConstraintsDelAll Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstraintsDelAll.html)

[IModelDoc2::ViewConstraint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ViewConstraint.html)

[IModelDoc2::SkToolsAutoConstr Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SkToolsAutoConstr.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0