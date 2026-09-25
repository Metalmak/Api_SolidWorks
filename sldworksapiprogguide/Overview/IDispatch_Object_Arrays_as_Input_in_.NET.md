<!-- source: sldworksapiprogguide/Overview/IDispatch_Object_Arrays_as_Input_in_.NET.htm -->

# SOLIDWORKS API Help

# IDispatch Object Arrays as Input in .NET

In the .NET Framework, an object array can be used to store System.Object
types like integer, double, etc. .NET marshals these data types automatically.
However, non-standard
object types like SOLIDWORKS interfaces must be explicitly marshaled to an
IDispatch object array.

Some SOLIDWORKS methods and properties have input arrays of non-standard objects.
Before passing these arrays, you must marshal them to IDispatch object arrays using
the System.Runtime.InteropServices.DispatchWrapper
class.

Several SOLIDWORKS methods and properties
have input object arrays that must be marshaled to an IDispatch object array.
The following Help topics contain links to VB.NET and C# examples that
demonstrate how to marshal
an array of non-standard input objects to an IDispatch object array.

* IAssemblyDoc::CopyWithMates
* IAssemblyDoc::ReorderComponents
* IExportPDFData::SetSheets
* ILibraryFeatureData::SetReferences
* ISheet::InsertTitleBlock
* IView::Bodies