<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~CheckSpelling.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CheckSpelling Method (IAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : CheckSpelling Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Options*
:   Spell-check options as defined in swCheckSpellingOptions\_e

*Dictionary*
:   :   Full path and filename of user dictionary to use (see **Remarks**)

Spell checks the text in this annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CheckSpelling( _    ByVal Options As System.Integer, _    ByVal Dictionary As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim Options As System.Integer Dim Dictionary As System.String Dim value As System.Object   value = instance.CheckSpelling(Options, Dictionary) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CheckSpelling(     System.int Options,    System.string Dictionary ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CheckSpelling(  &   System.int Options, &   System.String^ Dictionary ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Options*
:   Spell-check options as defined in swCheckSpellingOptions\_e

*Dictionary*
:   :   Full path and filename of user dictionary to use (see **Remarks**)

#### Return Value

Array of the misspelled words in this annotation

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::CheckSpelling.

# ![](dotnetimages/collapse.gif)Remarks

The SOLIDWORKS spell checker always uses a main dictionary, which is language specific. Use the Dictionary argument to specify an additional dictionary. If Dictionary is left blank, then no additional user dictionary is used.

You can also specify additional custom dictionaries by adding them in the appropriate location in the SOLIDWORKS registry.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15