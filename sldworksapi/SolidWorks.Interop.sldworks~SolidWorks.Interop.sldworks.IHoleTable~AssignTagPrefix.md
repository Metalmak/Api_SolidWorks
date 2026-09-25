<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~AssignTagPrefix.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AssignTagPrefix Method (IHoleTable) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html) : AssignTagPrefix Method (IHoleTable) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of row to which to apply TagPrefix

*TagPrefix*
:   Prefix to apply

*ApplyTo*
:   Apply to other holes as defined in swHoleTableTagPrefixApply\_e (see **Remarks**)

Prefixes the manual datum tags of specified holes with specified text.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AssignTagPrefix( _    ByVal Index As System.Integer, _    ByVal TagPrefix As System.String, _    ByVal ApplyTo As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHoleTable Dim Index As System.Integer Dim TagPrefix As System.String Dim ApplyTo As System.Integer Dim value As System.Boolean   value = instance.AssignTagPrefix(Index, TagPrefix, ApplyTo) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AssignTagPrefix(     System.int Index,    System.string TagPrefix,    System.int ApplyTo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AssignTagPrefix(  &   System.int Index, &   System.String^ TagPrefix, &   System.int ApplyTo ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index of row to which to apply TagPrefix

*TagPrefix*
:   Prefix to apply

*ApplyTo*
:   Apply to other holes as defined in swHoleTableTagPrefixApply\_e (see **Remarks**)

#### Return Value

True if prefix successfully assigned, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HoleTable::AssignTagPrefix.

# ![](dotnetimages/collapse.gif)Remarks

This method:

* is valid only if [IHoleTable::TagStyle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~TagStyle.html) is set to swHoleTableTagStyle\_e.swHoleTable\_ManualTags.* corresponds to the functionality of the **Assign Tag Prefix** dialog that pops up when you right-click on a hole table row of a manual tag.

If ApplyTo is specified with swHoleTableTagPrefixApply\_e:

* swHoleTableTagPrefixApply\_OnlySpecifiedHole, then only the hole as specified by Index is assigned TagPrefix.* swHoleTableTagPrefixApply\_AllHolesOfSameSize, then all holes that are the same size as the hole specified by Index are assigned TagPrefix.

When TagPrefix is assigned to only the hole as specified by Index, the numbering of all holes of the same size changes.

For example, if:

* A model view has six holes of two different sizes, and the hole table manual tags are initially labeled:

    AA1, AA2, AA3, AA4, BB1, BB2

* Specify Index with the row index of AA1.* Specify TagPrefix with "AB".* Specify ApplyTo with swHoleTableTagPrefixApply\_e.swHoleTableTagPrefixApply\_OnlySpecifiedHole.

After calling this method:

* The hole table manual tags are re-labeled:

    AB1, AA1, AA2, AA3, BB1, BB2

Notice that AA1 is re-labeled to AB1, and AA2 - AA4 are re-numbered to AA1 - AA3. BB1 and BB2 are unchanged.

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html)

[IHoleTable Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0