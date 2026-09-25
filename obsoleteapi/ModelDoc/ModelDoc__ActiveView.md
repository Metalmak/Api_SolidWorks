<!-- source: obsoleteapi/ModelDoc/ModelDoc__ActiveView.htm -->

# ModelDoc::ActiveView

This
property is obsolete and has been superseded byModelDoc2::ActiveView.

Description

This property returns the current active model view.

Syntax (OLE Automation)

ActiveView = ModelDoc.ActiveView (VB
Get property)

ActiveView = ModelDoc.GetActiveView
( ) (C++ Get property)

|  |  |  |
| --- | --- | --- |
| Property: | (LPDISPATCH) ActiveView | Pointer to a Dispatch object, the current active model view in this document |

Syntax
(Com)

status = ModelDoc->get\_IActiveView(
&ActiveView)

|  |  |  |
| --- | --- | --- |
| Property: | (LPMODELVIEW) ActiveView | Current active model view in this document |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks