<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~GetAttachedEntityTypes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAttachedEntityTypes Method (IAnnotation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html) : GetAttachedEntityTypes Method (IAnnotation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the types of entities attached to this annotation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAttachedEntityTypes() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAnnotation Dim value As System.Object   value = instance.GetAttachedEntityTypes() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetAttachedEntityTypes() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetAttachedEntityTypes(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of longs or integers (see Long vs. Integer) that indicate the attached entity types as defined in swSelectType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Annotation::GetAttachedEntityTypes.

# ![](dotnetimages/collapse.gif)Example

[Attach Annotation to Entity (C#)](Attach_Annotation_to_Entity_Example_CSharp.htm)

[Attach Annotation to Entity (VB.NET)](Attach_Annotation_to_Entity_Example_VBNET.htm)

[Attach Annotation to Entity (VBA)](Attach_Annotation_to_Entity_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supports all annotation types. Use [IAnnotation::GetType](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetType.html) to determine the annotation type.

This method returns an array of longs or integers indicating object types. The list of object types corresponds to the list of objects returned by [IAnnotation::GetAttachedEntities3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetAttachedEntities3.html).

You can associate annotations with additional items not listed in swSelectType\_e. If this annotation is attached to one or more entities not listed in swSelectType\_e, then this method and [IAnnotation::IGetAttachedEntityTypes](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~IGetAttachedEntityTypes.html) return swSelNOTHING in a position in the array corresponding to the unlisted item. IAnnotation::GetAttachedEntities3 indicates an unsupported entity by returning a null value in the position in the array corresponding to the unsupported entity. COM applications that call [IAnnotation::GetAttachedEntityCount3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAnnotation~GetAttachedEntityCount3.html) include the null value in the total count of associated entities.

If an annotation is disassociated from its geometry (i.e., dangling), then IAnnotation::GetAttachedEntities3 returns a null value in the position in the array corresponding to the dangling item, and this method returns swSelNOTHING in the position in the array corresponding to the dangling item.

NOTE: If this annotation is not associated with any geometry, then this method and IAnnotation::GetAttachedEntities3 return empty arrays.

# ![](dotnetimages/collapse.gif)See Also

####

[IAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation.html)

[IAnnotation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation_members.html)

[IAnnotation::SetAttachedEntities Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAnnotation~SetAttachedEntities.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207