<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertBendTable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBendTable Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : InsertBendTable Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X-coordinate for placement of the bend table

*Y*
:   Y-coordinate for placement of the bend table

*StartValue*
:   Starting datum tag; a value from A to Z for letter tags; a positive integer for number tags

*TableTemplate*
:   Full pathname of the template (e.g., *install\_dir*\**lang\***language**\*****bendtable-standard.sldbndtbt**)

Creates a bend table annotation for the flat pattern of this sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBendTable( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal StartValue As System.String, _    ByVal TableTemplate As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim X As System.Double Dim Y As System.Double Dim StartValue As System.String Dim TableTemplate As System.String Dim value As System.Object   value = instance.InsertBendTable(X, Y, StartValue, TableTemplate) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertBendTable(     System.double X,    System.double Y,    System.string StartValue,    System.string TableTemplate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertBendTable(  &   System.double X, &   System.double Y, &   System.String^ StartValue, &   System.String^ TableTemplate ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X-coordinate for placement of the bend table

*Y*
:   Y-coordinate for placement of the bend table

*StartValue*
:   Starting datum tag; a value from A to Z for letter tags; a positive integer for number tags

*TableTemplate*
:   Full pathname of the template (e.g., *install\_dir*\**lang\***language**\*****bendtable-standard.sldbndtbt**)

#### Return Value

[IBendTableAnnotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTableAnnotation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::InsertBendTable.

# ![](dotnetimages/collapse.gif)Example

'VBA

'\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

'1. Ensure the specified part and table template exist.
'2. Run the macro.
'3. Inserts a bend table annotation for the flat pattern.
'4. Inspect the graphics area and the Immediate window.

'\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Dim swApp As SldWorks.SldWorks
Dim myBendTableAnno As SldWorks.BendTableAnnotation
Dim myBendTable As SldWorks.BendTable
Dim Part As SldWorks.ModelDoc2
Dim boolstatus As Boolean
Dim longstatus As Long, longwarnings As Long
Option Explicit
Sub main()

> Set swApp = Application.SldWorks
> Set Part = swApp.OpenDoc6("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2019\samples\tutorial\api\SMGussetAPI.SLDPRT", 1, 0, "", longstatus, longwarnings)
> swApp.ActivateDoc2 "SMGussetAPI.SLDPRT", False, longstatus
> Set Part = swApp.ActiveDoc
>
> Set myBendTableAnno = Part.**InsertBendTable**(-4.06616963665726E-02, 6.09432383467686E-02, "A", "install\_dir\lang\english\bendtable-standard.sldbndtbt")
> Set myBendTable = myBendTableAnno.**BendTable**
> Debug.Print "Tag style of the bend table as defined in swBendTableTagStyle\_e: " & myBendTable.TagStyle
>
> End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

[IBendTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBendTable.html)

[IView::InsertBendTable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBendTable.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0