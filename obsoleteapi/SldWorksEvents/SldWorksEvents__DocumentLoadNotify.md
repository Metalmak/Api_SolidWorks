<!-- source: obsoleteapi/SldWorksEvents/SldWorksEvents__DocumentLoadNotify.htm -->

# DocumentLoadNotify - SldWorks Event

This event is obsolete and has been superseded
by SldWorksEvent::DocumentLoadNotify2.

Description

Post-notifies the user program
when a SolidWorks document is loaded.

NOTE:
If developing a C++ application, use swAppDocumentLoadNotify to register
for this notification.

status = DocumentLoadNotify ( docTitle , docPath
)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) docTitle | Document title |
| Input: | (BSTR) docPath | Document path |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

This event is fired for documents
referenced by assemblies and drawings. Client code should expect multiple
calls to this event handler when an assembly or drawing is loaded.