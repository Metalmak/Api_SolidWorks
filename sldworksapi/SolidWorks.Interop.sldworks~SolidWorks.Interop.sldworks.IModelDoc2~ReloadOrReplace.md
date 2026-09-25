<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ReloadOrReplace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReloadOrReplace Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : ReloadOrReplace Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ReadOnly*
:   True to set the model document read-only after reload or replace, false to allow write access

*ReplaceFileName*
:   Replacement model document; null or Nothing to reload the current model document

*DiscardChanges*
:   True to discard changes made to the current model document, false to abort operation if the model document was changed (see **Remarks**)

Obsolete. Superseded by [IModelDocExtension::ReloadOrReplace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ReloadOrReplace.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReloadOrReplace( _    ByVal ReadOnly As System.Boolean, _    ByVal ReplaceFileName As System.String, _    ByVal DiscardChanges As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim ReadOnly As System.Boolean Dim ReplaceFileName As System.String Dim DiscardChanges As System.Boolean Dim value As System.Integer   value = instance.ReloadOrReplace(ReadOnly, ReplaceFileName, DiscardChanges) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ReloadOrReplace(     System.bool ReadOnly,    System.string ReplaceFileName,    System.bool DiscardChanges ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ReloadOrReplace(  &   System.bool ReadOnly, &   System.String^ ReplaceFileName, &   System.bool DiscardChanges ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ReadOnly*
:   True to set the model document read-only after reload or replace, false to allow write access

*ReplaceFileName*
:   Replacement model document; null or Nothing to reload the current model document

*DiscardChanges*
:   True to discard changes made to the current model document, false to abort operation if the model document was changed (see **Remarks**)

#### Return Value

Error codes as defined by swComponentReloadError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::ReloadOrReplace.

# ![](dotnetimages/collapse.gif)Remarks

The model to reload or replace must be open in its own window frame.

This method does not reload or replace the model if the top assembly has been opened invisibly. In that case, make the model visible by calling [IModelDoc2::Visible](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~Visible.html) before calling this method.

You must call IModelDoc2::ReloadOrReplace after calling [IModelDoc2::ForceReleaseLocks](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ForceReleaseLocks.html), which detaches a file from the file system, to re-attach a detached file to the file system. If you do not call IModelDoc2::ReloadOrReplace after calling IModelDoc2::ForceReleaseLocks, then you will experience problems with OLE objects (e.g., design tables). Any changes made to a file while it is detached are not preserved unless you save the file to disk before calling IModelDoc2::ReloadOrReplace. Additionally if you set IModelDoc2::ReloadOrReplace's DiscardChanges parameter to false and you made changes to a detached file that you are attempting to re-attach to the file system, then IModelDoc2::ReloadOrReplace will fail. DiscardChanges must be set to true to re-attach a detached file.

See [ISldWorks::CloseAndReopen](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~CloseAndReopen.html) to perform a similar function with drawing documents.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IAssemblyDoc::ReplaceComponents Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ReplaceComponents.html)

[IAssemblyDoc::ComponentReload2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~ComponentReload2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0