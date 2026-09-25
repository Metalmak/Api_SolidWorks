<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetConstraints.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetConstraints Method (ISketchSegment) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html) : IGetConstraints Method (ISketchSegment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the constraints for this sketch segment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetConstraints() As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSegment Dim value As System.String   value = instance.IGetConstraints() ``` | |

| C# |  |
| --- | --- |
| ``` System.string IGetConstraints() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ IGetConstraints(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

* in-process, unmanaged C++: Pointer to an array of sketch segment constraints (see **Remarks**)

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Example

[Get Sketch Segment Constraints (C++)](Get_Sketch_Segment_Constraints_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

The available constraint values are as follows:

|  |  |  |
| --- | --- | --- |
| * sgHORIZONTAL * sgHORIZPOINTS * sgVERTICAL * sgVERTPOINTS * sgCOLINEAR * sgCORADIAL * sgPERPENDICULAR * sgPARALLEL * sgTANGENT * sgCONCENTRIC * sgCOINCIDENT | * sgSYMMETRIC * sgATMIDDLE * sgATINTERSECT * sgATPIERCE * sgFIXED  * sgANGLE * sgARCANG180 * sgARCANG270 * sgARCANG90 * sgARCANGBOTTOM * sgARCANGLEFT | * sgARCANGRIGHT * sgARCANGTOP * sgDIAMETER * sgDISTANCE * sgSAMELENGTH * sgOFFSETEDGE * sgSNAPANGLE * sgSNAPGRID * sgSNAPLENGTH * sgUSEEDGE * sgMERGEPOINTS |

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSegment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html)

[ISketchSegment::GetConstraints Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetConstraints.html)

[ISketchSegment::IGetConstraintsCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~IGetConstraintsCount.html)

[IModelDoc2::SketchConstraintsDelAll Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchConstraintsDelAll.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0