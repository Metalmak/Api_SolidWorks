<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| ISwAddin Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) : ISwAddin Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows applications to create SOLIDWORKS add-ins.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwAddin ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwAddin ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwAddin ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwAddin ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwAddin.

# ![](dotnetimages/collapse.gif)Remarks

To use this interface in a SOLIDWORKS VB.NET or C# macro or add-in, see ComVisibleAttribute in VB.NET and C# Macros and Add-ins.

If you are creating a COM-style addin and are using an MFC CCmdTarget-derived object to implement ISwAddin, you must fully implement ITypeInfo as follows:

* In the declaration of your CCmdTarget-derived class, add:

1. DECLARE\_OLETYPELIB(<your CCmdTarget-derived class name>)

   - \_\_declspec( dllexport ) virtual BOOL GetDispatchIID(IID\* pIID);

* In your implementation, add:

1. IMPLEMENT\_OLETYPELIB(<your class name>, LIBID\_SldWorks\_SWPublished, SOLIDWORKS\_type\_library\_version, 0)  //e.g., 14 for 2007

   - BOOL auAm\_c::GetDispatchIID(IID\* pIID)
     {

            \*pIID == IID\_ISwAddin;

            return True;

}

* In your class constructor, add:

 EnableTypeLib();

See also Using SwAddin to Create a SOLIDWORKS Add-in.

This interface is implemented by add-ins of SOLIDWORKS Partners who participate in the SOLIDWORKS Partner Program.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwAddin Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwAddin_members.html)

[SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html)