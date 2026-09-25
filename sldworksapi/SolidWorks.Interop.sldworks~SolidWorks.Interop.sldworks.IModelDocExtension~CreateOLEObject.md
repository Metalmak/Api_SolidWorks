<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~CreateOLEObject.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateOLEObject Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : CreateOLEObject Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Aspect*
:   Viewing aspect of the OLE object as defined in the DVASPECT enumeration (see **Remarks**)

*Position*
:   Top-left and bottom-right positions (see Remarks)

*Buffer*
:   Data for the OLE object (see Remarks)

*ErrorCode*
:   0 if True or 1 if false

Creates an OLE object on the active document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateOLEObject( _    ByVal Aspect As System.Integer, _    ByVal Position As System.Object, _    ByVal Buffer As System.Object, _    ByRef ErrorCode As System.Integer _ ) As SwOLEObject ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Aspect As System.Integer Dim Position As System.Object Dim Buffer As System.Object Dim ErrorCode As System.Integer Dim value As SwOLEObject   value = instance.CreateOLEObject(Aspect, Position, Buffer, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` SwOLEObject CreateOLEObject(     System.int Aspect,    System.object Position,    System.object Buffer,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SwOLEObject^ CreateOLEObject(  &   System.int Aspect, &   System.Object^ Position, &   System.Object^ Buffer, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Aspect*
:   Viewing aspect of the OLE object as defined in the DVASPECT enumeration (see **Remarks**)

*Position*
:   Top-left and bottom-right positions (see Remarks)

*Buffer*
:   Data for the OLE object (see Remarks)

*ErrorCode*
:   0 if True or 1 if false

#### Return Value

[OLE object](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISwOLEObject.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::CreateOLEObject.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **Argument** | **Information** |
| Aspect | Uses the DVASPECT enumeration, which has the following values:   * DVASPECT\_CONTENT = 1 * DVASPECT\_THUMBNAIL = 2 * DVASPECT\_ICON = 4 * DVASPECT\_DOCPRINT = 8   See the MSDN documentation for details about the DVASPECT enumeration. |
| Position | Specify:   * Sheet coordinates for drawings. * Screen pixel coordinates for parts and assemblies. |
| Buffer | See [ISwOLEObject::Buffer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISwOLEObject~Buffer.html) or specify [ISwOLEObject::IGetBuffer](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISwOLEObject~IGetBuffer.html)  - or - Get the data from your own OLE object.  The data is in the format obtained from the Microsoft MFC object COleClientItem using the GetHGlobalFromILockBytes. |

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetOLEObjectCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetOLEObjectCount.html)

[IModelDocExtension::GetOLEObjects Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetOLEObjects.html)

[IModelDocExtension::InsertObjectFromFile Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~InsertObjectFromFile.html)

[IModelDocExtension::ICreateOLEObject Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ICreateOLEObject.html)

[IModelDocExtension::IGetOLEObjects Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IGetOLEObjects.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0