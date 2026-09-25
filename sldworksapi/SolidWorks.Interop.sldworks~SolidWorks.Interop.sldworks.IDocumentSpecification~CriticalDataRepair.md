<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~CriticalDataRepair.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CriticalDataRepair Property (IDocumentSpecification) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDocumentSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html) : CriticalDataRepair Property (IDocumentSpecification) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to automatically repair critical data errors in the file to be opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CriticalDataRepair As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDocumentSpecification Dim value As System.Boolean   instance.CriticalDataRepair = value   value = instance.CriticalDataRepair ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CriticalDataRepair {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool CriticalDataRepair {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to automatically repair critical data errors, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DocumentSpecification::CriticalDataRepair.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [IDocumentSpecification::Silent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~Silent.html) is set to true.

If you set this property to true, and the file to open has critical data corruption:

* Critical data repair proceeds.* [ISldWorks::OpenDoc7](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~OpenDoc7.html) returns the document with warning, swFileLoadWarning\_e.swFileLoadWarning\_CriticalDataRepair.* All non-critical data errors are ignored, because repairing critical errors obliterates all non-critical data in the file.

If set to true, this property instructs SOLIDWORKS to repair critical data by importing Parasolid bodies into a new file. The repaired file contains only Parasolid bodies.

The following files are created in c**:\Users\***user***\AppData\Local\Temp:**

* **Repaired\_*file\_name.sld\***** **Backup of *file\_name.sld\****

If you set this property to false, and the file to open has critical data corruption:

* The document does not open.* ISldWorks::OpenDoc7 fails and returns null with error code, swFileLoadError\_e.FileRequiresCriticalDataRepair.

Use [IDocumentSpecification::AutoRepair](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~AutoRepair.html) to handle non-critical data corruption of files.

For C++ only, VARIANT\_TRUE (-1) automatically repairs the file, and VARIANT\_FALSE (0) does not.

# ![](dotnetimages/collapse.gif)See Also

####

[IDocumentSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html)

[IDocumentSpecification Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0