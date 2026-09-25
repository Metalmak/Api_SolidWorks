<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetObjectByPersistReference3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetObjectByPersistReference3 Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetObjectByPersistReference3 Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PersistId*
:   Object's persistent reference ID (see Remarks)

*ErrorCode*
:   Success or error code as defined by swPersistReferencedObjectStates\_e (see Remarks)

Gets the object assigned to the specified persistent reference ID.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetObjectByPersistReference3( _    ByVal PersistId As System.Object, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim PersistId As System.Object Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetObjectByPersistReference3(PersistId, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetObjectByPersistReference3(     System.object PersistId,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetObjectByPersistReference3(  &   System.Object^ PersistId, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PersistId*
:   Object's persistent reference ID (see Remarks)

*ErrorCode*
:   Success or error code as defined by swPersistReferencedObjectStates\_e (see Remarks)

#### Return Value

Object (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetObjectByPersistReference3.

# ![](dotnetimages/collapse.gif)Example

Sub main ()

    Set swApp = Application.SldWorks

    Set Doc = swApp.ActiveDoc
    Set SelMgr = Doc.SelectionManager
    If SelMgr.GetSelectedObjectCount(-1) = 0 Then Debug.Print "No selections found.": Exit Sub

    Dim persistRef As Variant
    Dim selObj As Object

    Set selObj = SelMgr.GetSelectedObject6(1, -1)
    persistRef = Doc.Extension.GetPersistReference3(selObj)
    Debug.Print UBound(persistRef)
    Set selObj = Nothing
    Set selObj = Doc.Extension.GetObjectByPersistReference3(persistRef, longstatus)
    Debug.Print (Not selObj Is Nothing)

    Dim selConfig As Configuration
    Set selConfig = selObj.GetSpecificFeature2

End Sub

# ![](dotnetimages/collapse.gif)Example

[Get Object's Persistent Reference ID (VBA)](Get_Object_s_Persistent_Reference_ID_Example_VB.htm)

[Use Persistent Reference (VBA)](Use_Persistent_Reference_Example_VB.htm)

[Use Persistent Reference (VB.NET)](Use_Persistent_Reference_Example_VBNET.htm)

[Use Persistent Reference (C#)](Use_Persistent_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A persistent reference ID is related to a model. It is portable and can be saved within the model or in other places. Some persistent reference IDs are general to all models and can be instantiated from all models. Your application must handle persistent reference IDs and their relationships among models.

Before calling this method, call [IModelDocExtension::GetPersistReference3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~GetPersistReference3.html) to get the object's persistent reference ID.

The swPersistReferencedObject\_Suppressed and swPersistReferencedObject\_Deleted enumerators only apply to references of topological entities.

IModelDocExtension::GetObjectByPersistReference3 was designed to return the base class of a feature to take advantage of the base feature class functionality. Objects returned by IModelDocExtension::GetObjectByPersistReference3 are often features, including [IConfiguration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IConfiguration.html), [IRefPlane](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefPlane.html), and [IRefAxis](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRefAxis.html) objects. You must first obtain a reference to a feature, and then use [IFeature::GetSpecificFeature2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetSpecificFeature2.html) to get the original object.

See Persistent Reference IDs for more information.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::IModelDocExtension::IGetObjectByPersistReference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IGetObjectByPersistReference3.html)

[IModelDocExtension::GetPersistReference3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetPersistReference3.html)

[IModelDocExtension::GetPersistReferenceCount3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetPersistReferenceCount3.html)

[IModelDocExtension::IsSamePersistentID Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~IsSamePersistentID.html)

[IView::ReferencedConfigurationID Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~ReferencedConfigurationID.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP3, Revision Number 15.3