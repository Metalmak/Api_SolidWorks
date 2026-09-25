<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~IFindMinimumRadius.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IFindMinimumRadius Method (ICurve) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : IFindMinimumRadius Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Bound*
:   Array containing the start and end boundary parameters (see **Remarks**)

*NumOfRadius*
:   Number of radius returned; can be 0 or 1

*Radius*
:   Minimum radius of curvature (see **Remarks**)

*Location*
:   [Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) where minimum radius curvature occurred  (see **Remarks**)

*Parameter*
:   Curve parameter  (see **Remarks**)

Finds the minimum radius of curvature of the selected curve and its position and u-v parameters.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IFindMinimumRadius( _    ByRef Bound As System.Double, _    ByRef NumOfRadius As System.Integer, _    ByRef Radius As System.Object, _    ByRef Location As System.Object, _    ByRef Parameter As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim Bound As System.Double Dim NumOfRadius As System.Integer Dim Radius As System.Object Dim Location As System.Object Dim Parameter As System.Object Dim value As System.Boolean   value = instance.IFindMinimumRadius(Bound, NumOfRadius, Radius, Location, Parameter) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IFindMinimumRadius(     ref System.double Bound,    out System.int NumOfRadius,    out System.object Radius,    out System.object Location,    out System.object Parameter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IFindMinimumRadius(  &   System.double% Bound, &   [Out] System.int NumOfRadius, &   [Out] System.Object^ Radius, &   [Out] System.Object^ Location, &   [Out] System.Object^ Parameter ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Bound*
:   Array containing the start and end boundary parameters (see **Remarks**)

*NumOfRadius*
:   Number of radius returned; can be 0 or 1

*Radius*
:   Minimum radius of curvature (see **Remarks**)

*Location*
:   [Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) where minimum radius curvature occurred  (see **Remarks**)

*Parameter*
:   Curve parameter  (see **Remarks**)

#### Return Value

True if operation succeeds, false if it fails

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::IFindMinimumRadius.

# ![](dotnetimages/collapse.gif)Example

**Unmanaged C++ COM:**

/////////////////////////////////////////////////////////////////////////////

// IMinRadius implementation

STDMETHODIMP CMinRadius::StartNotepad()

{

// TODO: Add your implementation code here

CComPtr<IModelDoc> iModelDoc2;

m\_iSldWorks->get\_**IActiveDoc**(&iModelDoc2);

CComPtr<ISelectionMgr> swSelMgr;

iModelDoc2->get\_**ISelectionManager**(&swSelMgr);

struct IDispatch\* pDispSelection;

CComPtr<IEdge> swEdge;

swSelMgr->**GetSelectedObject6**(1,-1,&pDispSelection);

pDispSelection->QueryInterface(

\_\_uuidof(IEdge),reinterpret\_cast<void\*\*>(&swEdge));

pDispSelection->Release();

double boundArr[2];

CComPtr<ICurve> swCurve;

swEdge->**IGetCurve**(&swCurve);

VARIANT\_BOOL isClose,isPeriodic,testRetVal;

swCurve->**GetEndParams**(&boundArr[0],&boundArr[1],&isClose,&isPeriodic,&testRetVal);

long numOfRadius(0);

VARIANT radius,Location,UVParameter;

VARIANT\_BOOL status(FALSE);

swCurve->**IFindMinimumRadius**(boundArr,&numOfRadius,&radius,&Location,&UVParameter,&status);

SafeDoubleArray radiusSA(radius);

double test1 = radiusSA[0];

SafeDISPATCHArray locationSA(Location);

CComPtr<IMathPoint> swMathPoint1;

locationSA[0]->QueryInterface(

\_\_uuidof(IMathPoint),reinterpret\_cast<void\*\*>(&swMathPoint1));

double locationArra1[3];

swMathPoint1->get\_**IArrayData**(locationArra1);

SafeDoubleArray UVParameterSA(UVParameter);

double uvpara1 = UVParameterSA[0];

return S\_OK;

}

# ![](dotnetimages/collapse.gif)Remarks

The search is confined to the portion of the selected curve lying inside of Bound.

COM returns these data types for these parameters:

* Radius: VARIANT of SafeDoubleArray* Location: VARIANT of SafeDispatchArray of [IMathpoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html)* Parameter: VARIANT of SafeDoubleArray

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[ICurve::FindMinimumRadius Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~FindMinimumRadius.html)

[ISurface::FindMinimumRadius Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~FindMinimumRadius.html)

[ISurface::IFindMinimumRadius Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface~IFindMinimumRadius.html)

[ICurve::GetEndParams Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~GetEndParams.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0