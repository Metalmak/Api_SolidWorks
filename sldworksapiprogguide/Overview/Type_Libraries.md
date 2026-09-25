<!-- source: sldworksapiprogguide/Overview/Type_Libraries.htm -->

# SOLIDWORKS API Help

# Type Libraries

This topic describes how to reference:

* [SOLIDWORKS type libraries](#SolidWorks)
* [User-specified type
  libraries](#User-specified)

## SOLIDWORKS Type Libraries

To reference the SOLIDWORKS type libraries, **sldworks.tlb** and **swconst.tlb**:

| If programming in... | Then... |
| Microsoft C++ 6.0 and Microsoft C++/CLI | In the precompiled header file, include:  #import "path\_and\_filename"  for each SOLIDWORKS type library that you are referencing. Path and filenames for each SOLIDWORKS type library are:  disk:\install\_dir\**sldworks.tlb**  disk:\install\_dir\**swconst.tlb** |
|  |  |
| Microsoft VBA | If you recorded a SOLIDWORKS macro, the SOLIDWORKS type libraries are automatically referenced.  - or -  To include the SOLIDWORKS type libraries manually:   1. In an open project in VBA, click Tools,    References. 2. Select:  * SldWorks   version   Type Library * SOLIDWORKS version   Constant type library        (Substitute the actual SOLIDWORKS version number for version.)  3. Click OK.   If a VBA macro created in an earlier version of SOLIDWORKS will not run after upgrading to a new version of SOLIDWORKS, see [VBA Macros, Type Libraries, and SOLIDWORKS Upgrades](VBA_Macros_Type_Libraries_and_SolidWorks_Upgrade.htm) for help. |
|  |  |
| Microsoft Visual Basic for Applications (VBA) | 1. In an open project in Visual Basic, click Project, References. 2. Select SOLIDWORKS    version Constant    type library.  3. Click OK. |

## User-specified Type Libraries

You can also add and remove references to user-specified type libraries.

* A user-specified type library first appears on
  the list of available references only after adding it and only after recording
  a macro.
* User-specified type library references are not
  persistent across SOLIDWORKS sessions.
* Only macros created after adding a user-specified
  type library reference can reference that type library.

See these topics for details about adding and removing references to
user-specified type libraries:

* ISldWorks::GetUserTypeLibReferenceCount
* ISldWorks::IGetUserTypeLibReferences
* ISldWorks::ISetUserTypeLibReferences
* ISldWorks::RemoveUserTypeLibReferences
* ISldWorks::UserTypeLibReferences