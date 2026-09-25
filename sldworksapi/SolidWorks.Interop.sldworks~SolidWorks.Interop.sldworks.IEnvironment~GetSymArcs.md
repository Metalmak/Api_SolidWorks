<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnvironment~GetSymArcs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSymArcs Method (IEnvironment) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnvironment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnvironment.html) : GetSymArcs Method (IEnvironment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SymId*
:   Name of the geometric tolerance symbol formatted as:

    <LibraryName-SymbolName>

    where LibraryName and SymbolName are a pre-defined SOLIDWORKS symbol in the SOLIDWORKS text file **gtol.sym**, typically installed at **C:\ProgramData\SolidWorks\SolidWorks 20***nn*\**lang**\**english****.**

    NOTE: You must include the right- and left-angle brackets and separate LibraryName and SymbolName with a hyphen; for example, <MOD-DEG>.

Obsolete. Superseded by [IEnvironment::GetSymArcs2.](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnvironment~GetSymArcs2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSymArcs( _    ByVal SymId As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnvironment Dim SymId As System.String Dim value As System.Object   value = instance.GetSymArcs(SymId) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetSymArcs(     System.string SymId ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetSymArcs(  &   System.String^ SymId ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SymId*
:   Name of the geometric tolerance symbol formatted as:

    <LibraryName-SymbolName>

    where LibraryName and SymbolName are a pre-defined SOLIDWORKS symbol in the SOLIDWORKS text file **gtol.sym**, typically installed at **C:\ProgramData\SolidWorks\SolidWorks 20***nn*\**lang**\**english****.**

    NOTE: You must include the right- and left-angle brackets and separate LibraryName and SymbolName with a hyphen; for example, <MOD-DEG>.

#### Return Value

Array (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Environment::GetSymArcs.

# ![](dotnetimages/collapse.gif)Remarks

Each arc in the geometric tolerance symbol is defined by three points (center, arc start, and end). The size of the array returned is based on the number of arcs within this geometric tolerance symbol. You can determine this number using the return value arc count from [IEnvironment::GetSymEdgeCounts](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnvironment~GetSymEdgeCounts.html).

The format of return value is the following array of doubles (in this example, for the *i*th arc):

retval[9 \* i + 0] = x coordinate of center point

retval[9 \* i + 1] = y coordinate of center point

retval[9 \* i + 2] = z coordinate of center point

retval[9 \* i + 3] = x coordinate of arc start point

retval[9 \* i + 4] = y coordinate of arc start point

retval[9 \* i + 5] = z coordinate of arc start point

retval[9 \* i + 6] = x coordinate of arc end point

retval[9 \* i + 7] = y coordinate of arc end point

retval[9 \* i + 8] = z coordinate of arc end point

# ![](dotnetimages/collapse.gif)See Also

####

[IEnvironment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnvironment.html)

[IEnvironment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnvironment_members.html)

[IEnvironment::IGetSymArcs Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnvironment~IGetSymArcs.html)