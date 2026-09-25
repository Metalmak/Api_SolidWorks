<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~GetExtremePoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetExtremePoint Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : GetExtremePoint Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X component of the direction vector

*Y*
:   Y component of the direction vector

*Z*
:   Z component of the direction vector

*Outx*
:   Extreme point X coordinate

*Outy*
:   Extreme point Y coordinate

*Outz*
:   Extreme point Z coordinate

Calculates the extreme point of the model in the specified direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetExtremePoint( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByRef Outx As System.Double, _    ByRef Outy As System.Double, _    ByRef Outz As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim Outx As System.Double Dim Outy As System.Double Dim Outz As System.Double Dim value As System.Boolean   value = instance.GetExtremePoint(X, Y, Z, Outx, Outy, Outz) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetExtremePoint(     System.double X,    System.double Y,    System.double Z,    out System.double Outx,    out System.double Outy,    out System.double Outz ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetExtremePoint(  &   System.double X, &   System.double Y, &   System.double Z, &   [Out] System.double Outx, &   [Out] System.double Outy, &   [Out] System.double Outz ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X component of the direction vector

*Y*
:   Y component of the direction vector

*Z*
:   Z component of the direction vector

*Outx*
:   Extreme point X coordinate

*Outy*
:   Extreme point Y coordinate

*Outz*
:   Extreme point Z coordinate

#### Return Value

True if a point was found, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::GetExtremePoint.

# ![](dotnetimages/collapse.gif)Remarks

This method returns the furthest possible point of intersection between a plane normal to the direction vector specified and the model as the plane moves along the direction vector. For example, if the model is a right cube centered on the origin and the direction vector is (1.0, 1.0, 1.0), then the extreme point is the vertex at (1.0,
1.0, 1.0).

If there is more than one point (for example, if there is a face perpendicular to the direction vector), SOLIDWORKS returns a unique point that it finds in a deterministic way.

**COM example**

HRESULT auBody\_c::XDispatch2::GetExtremePoint( double x, double y, double z, double\*
outx, double\* outy, double\* outz, VARIANT\_BOOL\* found ) {

> METHOD\_PROLOGUE\_EX\_(auBody\_c, Dispatch2)
>
> AU\_INTERFACE\_VERIFY\_NOT\_DISCONNECTED
>
> BOOL gotIt = pThis->GetExtremePoint(x, y, z, outx, outy, outz);
> \*found = gotIt ? VARIANT\_True : VARIANT\_false;
> return gotIt ? S\_OK : S\_false;

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0