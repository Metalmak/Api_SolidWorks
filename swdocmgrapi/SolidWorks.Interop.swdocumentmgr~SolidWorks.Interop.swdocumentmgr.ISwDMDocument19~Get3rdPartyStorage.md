<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19~Get3rdPartyStorage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| Get3rdPartyStorage Method (ISwDMDocument19) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDocument19 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19.html) : Get3rdPartyStorage Method (ISwDMDocument19) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StringIn*
:   Name of the stream; the name should be less than 30 characters and must be unique and qualified among all of the software parties storing within the current session

*IsStoring*
:   True if writing data, false if reading data

Gets an IStream interface to the specified third-party storage of this model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Get3rdPartyStorage( _    ByVal StringIn As System.String, _    ByVal IsStoring As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDocument19 Dim StringIn As System.String Dim IsStoring As System.Boolean Dim value As System.Object   value = instance.Get3rdPartyStorage(StringIn, IsStoring) ``` | |

| C# |  |
| --- | --- |
| ``` System.object Get3rdPartyStorage(     System.string StringIn,    System.bool IsStoring ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ Get3rdPartyStorage(  &   System.String^ StringIn, &   System.bool IsStoring ) ``` | |

#### Parameters

*StringIn*
:   Name of the stream; the name should be less than 30 characters and must be unique and qualified among all of the software parties storing within the current session

*IsStoring*
:   True if writing data, false if reading data

#### Return Value

Pointer to Unknown (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDocument19::Get3rdPartyStorage.

# ![](dotnetimages/collapse.gif)Example

[Read and Write to Third-party Storage (VB.NET)](Get_and_Set_3rd_Party_Storage_Example_VBNET.htm)

[Read and Write to Third-party Storage (C#)](Get_and_Set_3rd_Party_Storage_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you must call [ISwDMDocument19::Release3rdPartyStorage](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19~Release3rdPartyStorage.html). Otherwise, the third-party node might remain locked and prevent future access.

NOTE: The name given to the storage stream should be registered so that no conflicts occur. Once registered, the stream name is reserved exclusively for your application.

Passing the unique ID string and a flag to determine if data is being stored or loaded returns an IUnknown pointer. You must then use QueryInterface() to get the **Microsoft.VisualStudio.OLE.Interop.IStream** interface. The stream object is used for serialization and then released in the third-party code.

SwRootStorage --|

        |-- ThirdPty --|

                |-- <SW Assigned IStream name 1>

                |-- <SW Assigned IStream name 2>

                |-- <SW Assigned IStream name 3>

                ...

                |-- <SW Assigned IStream name *n*>

The IStream object used by the third party is written under an IStorage object called ThirdPty in the SOLIDWORKS compound document. Each third party writes to a single IStream object whose name is assigned by SOLIDWORKS.

NOTE: If you are using serialization, then be careful with the standard MFC macros. Otherwise, you may get a message like Unexpected File Format after your application is unloaded. One way of using IMPLEMENT\_SERIAL:

IMPLEMENT\_SERIAL( CCustomAttr, CObject, VERSIONABLE\_SCHEMA|0 )

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDocument19 Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19.html)

[ISwDMDocument19 Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19_members.html)

[ISwDMDocument19::Get3rdPartyStorageStore Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument19~Get3rdPartyStorageStore.html)

[ISwDMDocument20::Delete3rdPartyStorage Method ()](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDocument20~Delete3rdPartyStorage.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Document Manager API 2015 SP0