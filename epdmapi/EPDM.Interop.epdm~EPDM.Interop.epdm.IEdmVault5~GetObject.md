<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetObject Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : GetObject Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of object to get as defined in [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html)

*lObjectID*
:   ID of object to get

Gets an interface to a SOLIDWORKS PDM Professional object of the specified type and having the specified ID.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetObject( _    ByVal eType As EdmObjectType, _    ByVal lObjectID As System.Integer _ ) As IEdmObject5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmObject5 GetObject(     EdmObjectType eType,    System.int lObjectID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmObject5^ GetObject(  &   EdmObjectType eType, &   System.int lObjectID ) ``` | |

#### Parameters

*eType*
:   Type of object to get as defined in [EdmObjectType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmObjectType.html)

*lObjectID*
:   ID of object to get

#### Return Value

[IEdmObject5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmObject5.html)

# ![](dotnetimages/collapse.gif)Example

[Get File References for a File (C#)](Get_File_References_for_File_Example_CSharp.htm)

[Get File References for a File (VB.NET)](Get_File_References_for_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

As of SOLIDWORKS PDM Professional 2008 you can call [IEdmVault9::GetObjects](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault9~GetObjects.html) to get interfaces to several objects at once, which is more efficient than calling this method multiple times.

C++ users must release the returned pointer, IEdmObject5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_ID: The provided ID was not valid.* E\_EDM\_PERMISSION\_DENIED: The logged-in user does not have permission to see the requested object.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2