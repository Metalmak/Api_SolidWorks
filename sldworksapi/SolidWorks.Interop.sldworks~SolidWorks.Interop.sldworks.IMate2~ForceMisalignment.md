<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~ForceMisalignment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ForceMisalignment Method (IMate2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html) : ForceMisalignment Method (IMate2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Forces a misaligned mate condition for this concentric mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ForceMisalignment() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMate2 Dim value As System.Boolean   value = instance.ForceMisalignment() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ForceMisalignment() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ForceMisalignment(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if the misaligned mate condition is successfully created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mate2::ForceMisalignment.

# ![](dotnetimages/collapse.gif)Example

```
'VBA
```

```
' Open an assembly with a misaligned concentric mate, Concentric1
```

```
Dim swfeature As SldWorks.Feature
Dim swmate As SldWorks.Mate2
Sub main()
```

```
    Set swApp = Application.SldWorks
    Set swassm = swApp.ActiveDoc
    Set Swfeat = swassm.FeatureByName("Concentric1")
    Set swmate = Swfeat.GetSpecificFeature2
    Debug.Print "Concentric mate type as defined in swConcentricAlignmentType_e: " & swmate.GetConcentricAlignmentType
```

```
    'Remove the misaligned mate condition
    swmate.RemoveMisalignment

```

```
    'Create the misaligned mate condition
    swmate.ForceMisalignment
```

```
End Sub
```

# ![](dotnetimages/collapse.gif)See Also

####

[IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html)

[IMate2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2_members.html)

[IMate2::RemoveMisalignment Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~RemoveMisalignment.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0