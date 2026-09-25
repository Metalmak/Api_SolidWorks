<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISafeArrayUtility Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISafeArrayUtility Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Access the ISafeArrayUtility interface, which can:

* get an unpacked array of native SOLIDWORKS Dispatch-based objects of the same data type and return a packed Variant SafeArray to use in methods that requires passing a packed Variant SafeArray.* get a packed Variant SafeArray and return an unpacked array of native SOLIDWORKS Dispatch-based objects of the same data type.* get a Variant SafeArray and return the number of SafeArray objects in the Variant SafeArray and their data type.* get and put a value in a Variant SafeArray of the same data type.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISafeArrayUtility ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISafeArrayUtility ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISafeArrayUtility ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISafeArrayUtility ``` | |

# ![](dotnetimages/collapse.gif)Example

[Get Names of Configurations Using Variant (C++)](ConfigurationTraversalCPP.htm)

[Get Object's Persistent Reference ID (C++)](Get_Object_s_Persistent_Reference_ID_Example_CPlusPlus_COM.htm)

[Get Spline Points (C++)](Get_Spline_Points_Example_CPlusPlus_COM.htm)

[Get Scale Factor of Each Model View (C++)](Get_Scale_of_Each_Model_View_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)Remarks

The ISafeArrayUtility interface replaces the SOLIDWORKS SafeArray template class, which you might have used in earlier versions of SOLIDWORKS to instantiate SafeArrays for methods requiring Variant arrays in your C++ projects.

This ISafeArrayUtility interface's methods are only compatible with raw pointers and BSTRs; this interface's methods are not compatible with smart pointers (i.e., reference counted) or the Active Template Library (ATL) class CComBSTR. For example:

:   :   IDispatch\* pDisp1;  //This works:   IDispatchPtr pDisp2 //This does not work:   CComPtr<IDispatch> pDisp3 //This does not work
                :   BSTR fileName1 //This works:   CComBSTR fileName2 //This does not work

# ![](dotnetimages/collapse.gif)Accessors

[ISldWorks::GetSafeArrayUtility](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetSafeArrayUtility.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[SafeArrayUtility](SWObjectModel.pdf#SafeArrayUtility)

# ![](dotnetimages/collapse.gif)See Also

####

[ISafeArrayUtility Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)