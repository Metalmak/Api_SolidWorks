<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetStream.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetStream Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetStream Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StreamType*
:   1 = material stream

*ReadOnly*
:   True if the stream is read-only, false if not

Gets the handle for the specified stream.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetStream( _    ByVal StreamType As System.Integer, _    ByRef ReadOnly As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim StreamType As System.Integer Dim ReadOnly As System.Boolean Dim value As System.Object   value = instance.GetStream(StreamType, ReadOnly) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetStream(     System.int StreamType,    out System.bool ReadOnly ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetStream(  &   System.int StreamType, &   [Out] System.bool ReadOnly ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StreamType*
:   1 = material stream

*ReadOnly*
:   True if the stream is read-only, false if not

#### Return Value

Pointer to the IUnknown interface for this stream

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetStream.

# ![](dotnetimages/collapse.gif)Remarks

To release the stream, call [IModelDocExtension::ReleaseStream](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~ReleaseStream.html).

**VB Example**

This example illustrates attaching an XML document to a stream, and then releasing the stream.

Dim swApp As Object

Sub main()

Set swApp = Application.SldWorks

Dim docext As SldWorks.ModelDocExtension

Set docext = swApp.ActiveDoc.Extension

Dim xmldoc As MSXML2.DOMDocument

Set xmldoc = CreateObject("MSXML2.DOMDocument")

Dim stat As Boolean

Dim stream

Set stream = docext.GetStream(1, stat)

xmldoc.Load (stream)

docext.ReleaseStream (1)

xmldoc.Save ("C:\temp\xmlmat.xml")

End Sub

**C++ Example**

//--------

  CComPtr<IModelDocExtension> ext;

  m\_iModelDoc2->get\_Extension(&ext);

  LPSTREAM stream = NULL;

  VARIANT\_BOOL access = 0;

  ext->IGetStream(1, &access, &stream);

  // Your code

  if (stream)

  {

  VARIANT\_BOOL status;

  ext->IReleaseStream(1, &status);

  stream->Release();

  }

  //--------

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0