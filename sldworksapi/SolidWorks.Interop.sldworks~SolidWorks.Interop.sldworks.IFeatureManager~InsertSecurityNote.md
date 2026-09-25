<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSecurityNote.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSecurityNote Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSecurityNote Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Text*
:   Text for note

*FeatureOwner*
:   Macro feature for this note

Inserts a note for the specified [macro feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSecurityNote( _    ByVal Text As System.String, _    ByVal FeatureOwner As Feature _ ) As Note ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Text As System.String Dim FeatureOwner As Feature Dim value As Note   value = instance.InsertSecurityNote(Text, FeatureOwner) ``` | |

| C# |  |
| --- | --- |
| ``` Note InsertSecurityNote(     System.string Text,    Feature FeatureOwner ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Note^ InsertSecurityNote(  &   System.String^ Text, &   Feature^ FeatureOwner ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Text*
:   Text for note

*FeatureOwner*
:   Macro feature for this note

#### Return Value

Point to [INote](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.INote.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSecurityNote.

# ![](dotnetimages/collapse.gif)Remarks

The note is for display purposes only and cannot be modified by the end user. For example, you could display the note to inform an end user that editing or deleting the macro feature is prohibited.

You associate the note with the specified macro feature in:

* VB by using this method in the code that generates the macro feature and by setting swMacroFeatureSecurityEnableNote in the macro feature's security function. You should also include the conditions under which to display the note.

  * C++ by using this method in the code that generates the macro feature and by setting swMacroFeatureSecurityEnableNote for the Options argument of ISwComFeature::Security in the macro feature's security function. You should also include the conditions under which to display the note.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0