<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~PutBstr.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PutBstr Method (ISafeArrayUtility) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISafeArrayUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html) : PutBstr Method (ISafeArrayUtility) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VariantArray*
:   Variant SafeArray of BSTRs

*Index*
:   Index of BSTR

*Value*
:   BSTR

Adds the specified BSTR to a Variant SafeArray of BSTRs.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub PutBstr( _    ByRef VariantArray As System.Object, _    ByVal Index As System.Integer, _    ByVal Value As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISafeArrayUtility Dim VariantArray As System.Object Dim Index As System.Integer Dim Value As System.String   instance.PutBstr(VariantArray, Index, Value) ``` | |

| C# |  |
| --- | --- |
| ``` void PutBstr(     out System.object VariantArray,    System.int Index,    System.string Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void PutBstr(  &   [Out] System.Object^ VariantArray, &   System.int Index, &   System.String^ Value ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*VariantArray*
:   Variant SafeArray of BSTRs

*Index*
:   Index of BSTR

*Value*
:   BSTR

# ![](dotnetimages/collapse.gif)Remarks

Be aware that calling ISafeArrayUtility::PutBstr within a loop that inserts a BSTR repeatedly declared on the stack results in an array of pointers to the same BSTR; i.e., all elements of the SafeArray are the same, which is most likely not your intention. For example, you should avoid using code similar to the following:

for (ULONG ulIndex = 0L; ulIndex < ulSize; ulIndex++)
{
    CString testString;
    testString.Format(\_T('Index = %d'), ulIndex);
    CComBSTR bstrTemp = testString;
    HRESULT hres = iSAUtil->PutBstr(&vPacked, ulIndex, bstrTemp);

    bstrArray[ulIndex] = bstrTemp;
}

# ![](dotnetimages/collapse.gif)See Also

####

[ISafeArrayUtility Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility.html)

[ISafeArrayUtility Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility_members.html)

[ISafeArrayUtility::GetBstr Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISafeArrayUtility~GetBstr.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0