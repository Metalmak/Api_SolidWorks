<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAdvancedSelectionCriteria Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAdvancedSelectionCriteria Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to advanced component selection criteria for an assembly.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IAdvancedSelectionCriteria ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSelectionCriteria ``` | |

| C# |  |
| --- | --- |
| ``` public interface IAdvancedSelectionCriteria ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IAdvancedSelectionCriteria ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSelectionCriteria.

# ![](dotnetimages/collapse.gif)Example

'VBA

'-------------------------------------------------------
' Preconditions:
' 1. Open *Public\_Documents***\SOLIDWORKS\SOLIDWORKS 2021\samples\tutorial\advdrawings\98food processor.sldasm**.
' 2. Create **InContextHasMate.xml** with the following content:
'    <?xml version="1.0" encoding="UTF-8"?>
'    <SWQueryList>
'        <Query Name="InContextHasMate" Favourites\_Index="1">
'           <Boolean Name="And" Category="In Context Relations" SubCategory="Has mate to part" Condition="=" Value="base plate-1@98food processor"/>
'        </Query>
'    </SWQueryList>
' 3. Place **InContextHasMate.xml** in **c:\temp**.
' 4. Open the Immediate window.
'
' Postconditions: Inspect the Immediate window and the six selections
' in the FeatureManager design tree.
'-------------------------------------------------------
Option Explicit
Dim swAssem As SldWorks.AssemblyDoc
Dim criteria As SldWorks.AdvancedSelectionCriteria
Dim swApp As SldWorks.SldWorks
Dim Count As Long
Dim CriteriaFileName As String
Dim LoadSuccess As Boolean
Dim index As Long
Dim SelectSuccess As Boolean
Dim category1 As String
Dim category2 As String
Dim condition As Long
Dim val As String
Dim isAnd As Boolean

Sub main()

    Set swApp = Application.SldWorks
    Set swAssem = swApp.ActiveDoc
    Set criteria = swAssem.**GetAdvancedSelection**

    Count = criteria.GetItemCount
    Debug.Print "Before loading a query, GetItemCount returned " & Count

    ' Query file
    CriteriaFileName = "C:\temp\InContextHasMate.xml"

    ' Load query file
    LoadSuccess = criteria.**LoadCriteria**(CriteriaFileName)
    Debug.Print "Query " & CriteriaFileName & " load was" & IIf(LoadSuccess = False, " NOT ", " ") & "successful"

    Count = criteria.**GetItemCount**
    Debug.Print "After loading a query, GetItemCount returned " & Count

    For index = 0 To Count - 1
        If criteria.**GetItem2**(index, category1, category2, condition, val, isAnd) > -1 Then
            Debug.Print vbTab & " Criterion " & index & ": " & category1 & ", " & category2 & ", " & condition & ", " & val & ", " & isAnd
        Else
            Debug.Print vbTab & " Criterion " & index & " not found"
        End If
    Next

    Debug.Print swAssem.SelectionManager.GetSelectedObjectCount2(-1) & " objects selected before running query"

    ' Select components using selection criteria
    SelectSuccess = criteria.**Select**
    Debug.Print "Select was" & IIf(SelectSuccess = False, " NOT ", " ") & "successful"

    Debug.Print swAssem.SelectionManager.GetSelectedObjectCount2(-1) & " objects selected after running query"

End Sub

# ![](dotnetimages/collapse.gif)Example

[Select Assembly Components Using Advanced Selection Criteria (VB.NET)](Select_Assembly_Components_Using_Advanced_Selection_Criteria_Example_VBNET.htm)

[Select Assembly Components Using Advanced Selection Criteria (C#)](Select_Assembly_Components_Using_Advanced_Selection_Criteria_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface represents functionality in the Advanced Component Selection dialog that appears when you click **Standard toolbar > Advanced Select**.

As of SOLIDWORKS 2021, you can [save](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~SaveCriteria.html) criteria only in XML format. You can now [load](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria~LoadCriteria.html) either **\*.xml** queries or **\*.sqy** legacy queries.

For more information, see the **Assemblies > Basic Component Operations > Selecting Components > Advanced Component Selection** topic in the SOLIDWORKS user-interface help.

# ![](dotnetimages/collapse.gif)Accessors

[IAssemblyDoc::GetAdvancedSelection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~GetAdvancedSelection.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[AdvancedSelectionCriteria](SWObjectModel.pdf#AdvancedSelectionCriteria)

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSelectionCriteria Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSelectionCriteria_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)