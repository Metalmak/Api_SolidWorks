<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~PutDispatch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PutDispatch Method (ISafeArrayUtility) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISafeArrayUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html) : PutDispatch Method (ISafeArrayUtility) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VariantArray*
:   Variant SafeArray of Dispatch objects

*Index*
:   Index of Dispatch object

*Value*
:   Dispatch object

Adds the specified Dispatch object to a Variant SafeArray of Dispatch objects.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PutDispatch( _    ByRef VariantArray As System.Object, _    ByVal Index As System.Integer, _    ByVal Value As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISafeArrayUtility Dim VariantArray As System.Object Dim Index As System.Integer Dim Value As System.Object   instance.PutDispatch(VariantArray, Index, Value) ``` | |

| C# |  |
| --- | --- |
| ``` void PutDispatch(     out System.object VariantArray,    System.int Index,    System.object Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PutDispatch(  &   [Out] System.Object^ VariantArray, &   System.int Index, &   System.Object^ Value ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VariantArray*
:   Variant SafeArray of Dispatch objects

*Index*
:   Index of Dispatch object

*Value*
:   Dispatch object

# ![](dotnetimages/collapse.gif)See Also

####

[ISafeArrayUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html)

[ISafeArrayUtility Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility_members.html)

[ISafeArrayUtility::GetDispatch Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~GetDispatch.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0