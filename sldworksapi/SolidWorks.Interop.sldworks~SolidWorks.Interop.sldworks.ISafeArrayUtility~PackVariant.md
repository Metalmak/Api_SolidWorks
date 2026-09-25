<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~PackVariant.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PackVariant Method (ISafeArrayUtility) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISafeArrayUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html) : PackVariant Method (ISafeArrayUtility) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VariantArray*
:   Packed Variant SafeArray

*Count*
:   Number of native SOLIDWORKS Dispatch-based objects of Type

*Type*
:   Data type as defined in swSafeArrayType\_e

*Data*
:   Native SOLIDWORKS Dispatch-based objects of Type

Packs the specified native SOLIDWORKS Dispatch-based objects of the same data type into a Variant SafeArray and returns that packed Variant SafeArray to use in methods requiring passing a packed Variant SafeArray.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PackVariant( _    ByRef VariantArray As System.Object, _    ByVal Count As System.Integer, _    ByVal Type As System.Integer, _    ByRef Data As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISafeArrayUtility Dim VariantArray As System.Object Dim Count As System.Integer Dim Type As System.Integer Dim Data As System.Integer   instance.PackVariant(VariantArray, Count, Type, Data) ``` | |

| C# |  |
| --- | --- |
| ``` void PackVariant(     out System.object VariantArray,    System.int Count,    System.int Type,    ref System.int Data ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PackVariant(  &   [Out] System.Object^ VariantArray, &   System.int Count, &   System.int Type, &   System.int% Data ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VariantArray*
:   Packed Variant SafeArray

*Count*
:   Number of native SOLIDWORKS Dispatch-based objects of Type

*Type*
:   Data type as defined in swSafeArrayType\_e

*Data*
:   Native SOLIDWORKS Dispatch-based objects of Type

# ![](dotnetimages/collapse.gif)Example

[Get Scale Factor of Each Model View (C++)](Get_Scale_of_Each_Model_View_Example_CPlusPlus_COM.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISafeArrayUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html)

[ISafeArrayUtility Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility_members.html)

[ISafeArrayUtility::GetInfo Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~GetInfo.html)

[ISafeArrayUtility::UnPackVariant Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~UnPackVariant.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0