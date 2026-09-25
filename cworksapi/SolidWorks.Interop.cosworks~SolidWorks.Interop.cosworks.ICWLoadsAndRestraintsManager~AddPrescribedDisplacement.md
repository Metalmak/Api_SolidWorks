<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddPrescribedDisplacement.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddPrescribedDisplacement Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddPrescribedDisplacement Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Displacements*
:   Array: [*disp\_x\_coord*, *disp\_y\_coord*, *disp\_z\_coord*, *x\_bool*, *y\_bool*, *z\_bool*]

    where:

    | Array Element | Value | Description |
    | --- | --- | --- |
    | *disp\_x\_coord* | Double | Prescribed displacement in the x direction |
    | *disp\_y\_coord* | Double | Prescribed displacement in the y direction |
    | *disp\_z\_coord* | Double | Prescribed displacement in the z direction |
    | *x\_bool* | 0 or 1 | Whether to use *disp\_x\_coord* (1 to use*,* 0 to not) |
    | *y\_bool* | 0 or 1 | Whether to use *disp\_y\_coord* (1 to use*,* 0 to not) |
    | *z\_bool* | 0 or 1 | Whether to use *disp\_z\_coord* (1 to use*,* 0 to not) |

    (see **Remarks**)

*NLengthUnit*
:   Units of length as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

*DispArray*
:   Array of entities to which to apply the prescribed displacement specified in Displacements

*RefGeom*
:   Reference entity for prescribed displacement direction

*ErrorCode*
:   Error code as defined in [swsRestraintError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRestraintError_e.html)

Applies the specified prescribed displacement to the specified geometric entities to create a fixture.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddPrescribedDisplacement( _    ByVal Displacements As System.Object, _    ByVal NLengthUnit As System.Integer, _    ByVal DispArray As System.Object, _    ByVal RefGeom As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWRestraint ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim Displacements As System.Object Dim NLengthUnit As System.Integer Dim DispArray As System.Object Dim RefGeom As System.Object Dim ErrorCode As System.Integer Dim value As CWRestraint   value = instance.AddPrescribedDisplacement(Displacements, NLengthUnit, DispArray, RefGeom, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWRestraint AddPrescribedDisplacement(     System.object Displacements,    System.int NLengthUnit,    System.object DispArray,    System.object RefGeom,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWRestraint^ AddPrescribedDisplacement(  &   System.Object^ Displacements, &   System.int NLengthUnit, &   System.Object^ DispArray, &   System.Object^ RefGeom, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*Displacements*
:   Array: [*disp\_x\_coord*, *disp\_y\_coord*, *disp\_z\_coord*, *x\_bool*, *y\_bool*, *z\_bool*]

    where:

    | Array Element | Value | Description |
    | --- | --- | --- |
    | *disp\_x\_coord* | Double | Prescribed displacement in the x direction |
    | *disp\_y\_coord* | Double | Prescribed displacement in the y direction |
    | *disp\_z\_coord* | Double | Prescribed displacement in the z direction |
    | *x\_bool* | 0 or 1 | Whether to use *disp\_x\_coord* (1 to use*,* 0 to not) |
    | *y\_bool* | 0 or 1 | Whether to use *disp\_y\_coord* (1 to use*,* 0 to not) |
    | *z\_bool* | 0 or 1 | Whether to use *disp\_z\_coord* (1 to use*,* 0 to not) |

    (see **Remarks**)

*NLengthUnit*
:   Units of length as defined in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html)

*DispArray*
:   Array of entities to which to apply the prescribed displacement specified in Displacements

*RefGeom*
:   Reference entity for prescribed displacement direction

*ErrorCode*
:   Error code as defined in [swsRestraintError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRestraintError_e.html)

#### Return Value

[ICWRestraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRestraint.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddPrescribedDisplacement.

# ![](dotnetimages/collapse.gif)Example

[Add Prescribed Displacement (VBA)](Add_Prescribed_Displacement_Example_VB.htm)

[Add Prescribed Displacement (VB.NET)](Add_Prescribed_Displacement_Example_VBNET.htm)

[Add Prescribed Displacement (C#)](Add_Prescribed_Displacement_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The Displacements parameter specifies:

* length for reference geometry or flat faces

   - or -

* angle of rotation for cylindrical or spherical faces

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP3