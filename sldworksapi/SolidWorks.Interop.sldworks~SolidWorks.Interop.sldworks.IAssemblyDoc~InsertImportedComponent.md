<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~InsertImportedComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertImportedComponent Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : InsertImportedComponent Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Full path name of the third-party native CAD file to insert

*X*
:   X-coordinate of the component center

*Y*
:   Y-coordinate of the component center

*Z*
:   Z-coordinate of the component center

*CompInserted*
:   [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html); null or Nothing if unsuccessful

Inserts a third-party native CAD part or assembly into the current configuration of this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertImportedComponent( _    ByVal FileName As System.String, _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByRef CompInserted As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim FileName As System.String Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim CompInserted As System.Object Dim value As System.Integer   value = instance.InsertImportedComponent(FileName, X, Y, Z, CompInserted) ``` | |

| C# |  |
| --- | --- |
| ``` System.int InsertImportedComponent(     System.string FileName,    System.double X,    System.double Y,    System.double Z,    out System.object CompInserted ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int InsertImportedComponent(  &   System.String^ FileName, &   System.double X, &   System.double Y, &   System.double Z, &   [Out] System.Object^ CompInserted ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Full path name of the third-party native CAD file to insert

*X*
:   X-coordinate of the component center

*Y*
:   Y-coordinate of the component center

*Z*
:   Z-coordinate of the component center

*CompInserted*
:   [IComponent2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html); null or Nothing if unsuccessful

#### Return Value

Error code as defined in sw3DInterconnectImportErrors\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::InsertImportedComponent.

# ![](dotnetimages/collapse.gif)Remarks

To successfully use this method, you must first turn on 3D Interconnect by either:

* Setting **Tools > Options > System Options > Import > Enable 3D Interconnect**

    - or -

* Calling [ISldWorks::SetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html)(swUserPreferenceToggle\_e.swMultiCAD\_Enable3DInterconnect, True)

To edit the imported assembly, save the SOLIDWORKS assembly and then use [IFeature::GetImportedFeatureParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetImportedFeatureParameters.html) and [IFeature::SetImportedFeatureParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetImportedFeatureParameters.html).

See the [IImport3DInterconnectData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImport3DInterconnectData.html) Remarks.

If 3D Interconnect is turned off, use [IAssemblyDoc::AddComponent5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddComponent5.html) instead of this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[ISldWorks::LoadFile4 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~LoadFile4.html)

[IPartDoc::InsertImportedFeature Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertImportedFeature.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0