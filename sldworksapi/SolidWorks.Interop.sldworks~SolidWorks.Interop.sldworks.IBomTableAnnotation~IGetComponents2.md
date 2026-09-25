<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetComponents2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetComponents2 Method (IBomTableAnnotation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html) : IGetComponents2 Method (IBomTableAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RowIndex*
:   Row in the BOM table where to get the components; 0-based index

*Configuration*
:   Configuration for which to count components in top-level only BOMs; specify an empty string for parts only and indented BOMs

*Count*
:   Number of components in the specified row

Gets the components in the specified row for the specified configuration in this BOM table annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetComponents2( _    ByVal RowIndex As System.Integer, _    ByVal Configuration As System.String, _    ByVal Count As System.Integer _ ) As Component2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBomTableAnnotation Dim RowIndex As System.Integer Dim Configuration As System.String Dim Count As System.Integer Dim value As Component2   value = instance.IGetComponents2(RowIndex, Configuration, Count) ``` | |

| C# |  |
| --- | --- |
| ``` Component2 IGetComponents2(     System.int RowIndex,    System.string Configuration,    System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Component2^ IGetComponents2(  &   System.int RowIndex, &   System.String^ Configuration, &   System.int Count ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RowIndex*
:   Row in the BOM table where to get the components; 0-based index

*Configuration*
:   Configuration for which to count components in top-level only BOMs; specify an empty string for parts only and indented BOMs

*Count*
:   Number of components in the specified row

#### Return Value

* in-process, unmanaged C++: Pointer to an array of [components](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) in the specified row for the specified configuration

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IBomTableAnnotation::GetComponentsCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~GetComponentsCount2.html) to get the value of Count.

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[IBomTableAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html)

[IBomTableAnnotation::GetComponents2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetComponents2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 SP03 , Revision Number 19.3