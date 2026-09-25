<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetGridSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetGridSettings Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : GetGridSettings Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the current grid settings.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetGridSettings() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim value As System.Object   value = instance.GetGridSettings() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetGridSettings() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetGridSettings(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Current grid settings (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::GetGridSettings.

# ![](dotnetimages/collapse.gif)Remarks

The return format is the following array of doubles:

[ dispGrid, gridSpacing, snap, dotStyle, nMajor, nMinor, angleSnap, angleUnit, minorAuto ]

where:

* dispGrid - can be interpreted as a BOOLEAN: True if grid displayed, false otherwise

  * gridSpacing - snap distance

    * snap - can be interpreted as a BOOLEAN: True if snap to grid is on, false otherwise

      * dotStyle - can be interpreted as a BOOLEAN: True if dotted grids, false otherwise

        * nMajor - number of minors in major

          * nMinor - number of snaps in minor

            * angleSnap - can be interpreted as a BOOLEAN: True if snap to angle is on, false otherwise

              * angleUnit - value of angle to which to snap

                * minorAuto - an be interpreted as a BOOLEAN: True if the minor grids are set automatically, false otherwise

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::GridOptions Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GridOptions.html)

[IModelDoc2::ToolsGrid Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ToolsGrid.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0