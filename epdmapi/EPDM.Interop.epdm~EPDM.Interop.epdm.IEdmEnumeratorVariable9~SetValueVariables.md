<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable9~SetValueVariables.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetValueVariables Method (IEdmEnumeratorVariable9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVariable9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable9.html) : SetValueVariables Method (IEdmEnumeratorVariable9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVarNamesList*
:   [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html); list of variable names

*poVarValuesList*
:   [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html); list of values for variable names in poVarNamesList

*bsCfgName*
:   Configuration name

*bOnlyIfPartOfCard*
:   True to set the variable only if the variable is part of the data card, false to always set the variable (see **Remarks**)

Sets the values of file variables.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetValueVariables( _    ByVal poVarNamesList As EdmStrLst5, _    ByVal poVarValuesList As EdmStrLst5, _    ByVal bsCfgName As System.String, _    Optional ByVal bOnlyIfPartOfCard As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetValueVariables(     EdmStrLst5 poVarNamesList,    EdmStrLst5 poVarValuesList,    System.string bsCfgName,    System.bool bOnlyIfPartOfCard ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetValueVariables(  &   EdmStrLst5^ poVarNamesList, &   EdmStrLst5^ poVarValuesList, &   System.String^ bsCfgName, &   System.bool bOnlyIfPartOfCard ) ``` | |

#### Parameters

*poVarNamesList*
:   [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html); list of variable names

*poVarValuesList*
:   [IEdmStrLst5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmStrLst5.html); list of values for variable names in poVarNamesList

*bsCfgName*
:   Configuration name

*bOnlyIfPartOfCard*
:   True to set the variable only if the variable is part of the data card, false to always set the variable (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

This method can write the value to the file if the variable is mapped to a custom property.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVariable9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable9.html)

[IEdmEnumeratorVariable9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVariable9_members.html)