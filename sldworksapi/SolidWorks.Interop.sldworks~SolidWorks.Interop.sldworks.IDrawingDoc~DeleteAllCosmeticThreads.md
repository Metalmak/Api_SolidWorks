<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~DeleteAllCosmeticThreads.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DeleteAllCosmeticThreads Method (IDrawingDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html) : DeleteAllCosmeticThreads Method (IDrawingDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Deletes all cosmetic threads, which do not have callouts, in a drawing of an assembly only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub DeleteAllCosmeticThreads() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDrawingDoc   instance.DeleteAllCosmeticThreads() ``` | |

| C# |  |
| --- | --- |
| ``` void DeleteAllCosmeticThreads() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DeleteAllCosmeticThreads(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DrawingDoc::DeleteAllCosmeticThreads.

# ![](dotnetimages/collapse.gif)Example

**VB.NET:**

'---------------------------------------------------

'

' Preconditions: Drawing of an assembly with

' cosmetic threads is active.

'

' Postconditions: Cosmetic threads without callouts

' are deleted.

'

'---------------------------------------------------

Option

 Explicit On

Imports SOLIDWORKS.Interop.sldworks

Imports

 SOLIDWORKS.Interop.swconst

Imports

 System

Partial

 Class SOLIDWORKSMacro
> Public Sub main()
>
> > Dim swDrawingDoc As DrawingDoc
> >
> > Dim swModel As ModelDoc2
> >
> > Dim boolstatus As Boolean
> >
> >
> >
> > swDrawingDoc = swApp.ActiveDoc
> >
> > swDrawingDoc.DeleteAllCosmeticThreads()
> >
> > swModel = swDrawingDoc
> >
> > boolstatus = swModel.ForceRebuild3(False)
>
> End Sub
>
>
>
> ''' <summary>
>
> ''' The SldWorks swApp variable is pre-assigned for you.
>
> ''' </summary>
>
> Public swApp As SldWorks

End

 Class

# ![](dotnetimages/collapse.gif)Remarks

This method only deletes cosmetic threads in a drawing of an assembly; this method does not delete cosmetic threads in a drawing of a part.

By default, cosmetic threads are not imported into an drawing of an assembly for performance reasons, but are imported into a drawing of part and belong to the features in the part; thus, they cannot be deleted using this method.

This method also does not delete any cosmetic threads with callouts in a drawing of an assembly.

# ![](dotnetimages/collapse.gif)See Also

####

[IDrawingDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc.html)

[IDrawingDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc_members.html)

[ICThread Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICThread.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP2, Revision Number 17.2