<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SetLightSourcePropertyValuesVB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLightSourcePropertyValuesVB Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SetLightSourcePropertyValuesVB Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*IdName*

*LType*

*Diff*

*RgbColor*

*Dist*

*DirX*

*DirY*

*DirZ*

*SpotDirX*

*SpotDirY*

*SpotDirZ*

*SpotAngle*

*FallOff0*

*FallOff1*

*FallOff2*

*Ambient*

*Specular*

*SpotExponent*

*BDisable*

Obsolete. Superseded by [IModelDoc2::SetLightSourcePropertyValuesVB](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SetLightSourcePropertyValuesVB.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLightSourcePropertyValuesVB( _    ByVal IdName As System.String, _    ByVal LType As System.Integer, _    ByVal Diff As System.Double, _    ByVal RgbColor As System.Integer, _    ByVal Dist As System.Double, _    ByVal DirX As System.Double, _    ByVal DirY As System.Double, _    ByVal DirZ As System.Double, _    ByVal SpotDirX As System.Double, _    ByVal SpotDirY As System.Double, _    ByVal SpotDirZ As System.Double, _    ByVal SpotAngle As System.Double, _    ByVal FallOff0 As System.Double, _    ByVal FallOff1 As System.Double, _    ByVal FallOff2 As System.Double, _    ByVal Ambient As System.Double, _    ByVal Specular As System.Double, _    ByVal SpotExponent As System.Double, _    ByVal BDisable As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim IdName As System.String Dim LType As System.Integer Dim Diff As System.Double Dim RgbColor As System.Integer Dim Dist As System.Double Dim DirX As System.Double Dim DirY As System.Double Dim DirZ As System.Double Dim SpotDirX As System.Double Dim SpotDirY As System.Double Dim SpotDirZ As System.Double Dim SpotAngle As System.Double Dim FallOff0 As System.Double Dim FallOff1 As System.Double Dim FallOff2 As System.Double Dim Ambient As System.Double Dim Specular As System.Double Dim SpotExponent As System.Double Dim BDisable As System.Boolean Dim value As System.Boolean   value = instance.SetLightSourcePropertyValuesVB(IdName, LType, Diff, RgbColor, Dist, DirX, DirY, DirZ, SpotDirX, SpotDirY, SpotDirZ, SpotAngle, FallOff0, FallOff1, FallOff2, Ambient, Specular, SpotExponent, BDisable) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetLightSourcePropertyValuesVB(     System.string IdName,    System.int LType,    System.double Diff,    System.int RgbColor,    System.double Dist,    System.double DirX,    System.double DirY,    System.double DirZ,    System.double SpotDirX,    System.double SpotDirY,    System.double SpotDirZ,    System.double SpotAngle,    System.double FallOff0,    System.double FallOff1,    System.double FallOff2,    System.double Ambient,    System.double Specular,    System.double SpotExponent,    System.bool BDisable ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetLightSourcePropertyValuesVB(  &   System.String^ IdName, &   System.int LType, &   System.double Diff, &   System.int RgbColor, &   System.double Dist, &   System.double DirX, &   System.double DirY, &   System.double DirZ, &   System.double SpotDirX, &   System.double SpotDirY, &   System.double SpotDirZ, &   System.double SpotAngle, &   System.double FallOff0, &   System.double FallOff1, &   System.double FallOff2, &   System.double Ambient, &   System.double Specular, &   System.double SpotExponent, &   System.bool BDisable ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*IdName*

*LType*

*Diff*

*RgbColor*

*Dist*

*DirX*

*DirY*

*DirZ*

*SpotDirX*

*SpotDirY*

*SpotDirZ*

*SpotAngle*

*FallOff0*

*FallOff1*

*FallOff2*

*Ambient*

*Specular*

*SpotExponent*

*BDisable*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SetLightSourcePropertyValuesVB.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)