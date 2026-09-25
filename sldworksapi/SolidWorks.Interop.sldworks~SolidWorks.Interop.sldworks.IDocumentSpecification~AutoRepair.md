<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~AutoRepair.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AutoRepair Property (IDocumentSpecification) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDocumentSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html) : AutoRepair Property (IDocumentSpecification) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to automatically repair non-critical custom properties errors in the file to be opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AutoRepair As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDocumentSpecification Dim value As System.Boolean   instance.AutoRepair = value   value = instance.AutoRepair ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AutoRepair {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool AutoRepair {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to automatically repair custom properties errors, false to not (default) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DocumentSpecification::AutoRepair.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [IDocumentSpecification::Silent](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~Silent.html) is set to true.

If the document to be opened has a non-critical data error, the non-critical data error may or may not be repaired, depending on how you set this property and other conditions.

If you set this property to true, and the file to open has non-critical data corruption in:

* The custom properties area, the repair proceeds, and [ISldWorks::OpenDoc7](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~OpenDoc7.html) returns the document with warning, swFileLoadWarning\_e.swFileLoadWarning\_AutomaticRepair.* An area other than custom properties, the document is not repaired.

The following files are created in c**:\Users\***user***\AppData\Local\Temp:**

* **Repaired\_*file\_name.sld\***** **Backup of *file\_name.sld\****

If you set this property to false, and the file to open has non-critical data corruption:

* The document is not repaired.* The document does not open.* [ISldWorks::OpenDoc7](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~OpenDoc7.html) fails and returns null with error code, swFileLoadError\_e.FileRequiresAutoRepair.

If critical data corruption exists in the file, and you set [IDocumentSpecification::CriticalDataRepair](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification~CriticalDataRepair.html) to true to handle critical data corruption:

* Non-critical data corruptions are ignored and not repaired.* Repairing critical errors necessitates obliterating all non-critical data.

Use For C++ only, VARIANT\_TRUE (-1) automatically repairs the file, and VARIANT\_FALSE (0) does not.

# ![](dotnetimages/collapse.gif)See Also

####

[IDocumentSpecification Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification.html)

[IDocumentSpecification Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDocumentSpecification_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0