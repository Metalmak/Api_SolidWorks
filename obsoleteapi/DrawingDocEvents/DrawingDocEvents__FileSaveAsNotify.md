<!-- source: obsoleteapi/DrawingDocEvents/DrawingDocEvents__FileSaveAsNotify.htm -->

# FileSaveAsNotify - DrawingDoc Event

This event is obsolete and has been superseded
by the DrawingDoc event FileSaveAsNotify2.

Description

Pre-notifies the user program
when a file is about to be saved with a new name and passes the new document
name.

status = FileSaveAsNotify ( FileName )

| Input: | (BSTR) FileName | Name of the saved file |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

You might want to check the file extension on FileName
because the user might be saving this document as IGES, DXF, and so on.
When a user selects File, Save for a document that has never
been saved, SolidWorks generates FileSaveAsNotify instead of FileSaveNotify.
Return S\_FALSE to stop
SolidWorks from proceeding with the action that caused the notification.