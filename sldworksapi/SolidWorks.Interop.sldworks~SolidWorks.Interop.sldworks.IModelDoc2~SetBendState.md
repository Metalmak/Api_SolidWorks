<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetBendState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBendState Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SetBendState Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BendState*
:   Sheet metal state to set in this part as defined in swSMBendState\_e

Sets the bend state of a sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBendState( _    ByVal BendState As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim BendState As System.Integer Dim value As System.Integer   value = instance.SetBendState(BendState) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetBendState(     System.int BendState ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetBendState(  &   System.int BendState ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BendState*
:   Sheet metal state to set in this part as defined in swSMBendState\_e

#### Return Value

Status of the set operation as defined in swSMCommandStatus\_e (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SetBendState.

# ![](dotnetimages/collapse.gif)Example

[Flatten Sheet Metal Part (VBA)](Flatten_Sheet_Metal_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only works for old-style sheet metal parts or non-sheet metal parts converted to sheet metal parts. To set the bend state on new-style sheet metal parts (i.e., those that have a base flange as their first feature), suppress and unsuppress the flat-pattern feature.

If editing a part with bend information in the context of the assembly (see [IAssemblyDoc::EditPart2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~EditPart2.html)), the bend state for that part will be set.

|  |  |
| --- | --- |
| **If this method is executed on...** | **Then...** |
| Part without bend information | The part is not affected, and retval is set to swSMErrorNotASheetMetalPart |
| Assembly | The assembly is not affected, and retval is set to swSMErrorNotAPart |
| NOTE:  In both of these cases, status is S\_false for the COM version of this method. | |

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GetBendState Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetBendState.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0