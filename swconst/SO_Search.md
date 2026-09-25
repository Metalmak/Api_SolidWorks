<!-- source: swconst/SO_Search.htm -->

# SOLIDWORKS API Help

# System Options > Search

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture corresponds to the settings on that dialog.
* titled [Obsolete
  Enumerators](#Obsolete) contains enumerators that previously appeared on the dialog
  but are now obsolete.

The Search dialog is not available in SOLIDWORKS Connected.

![](SO_Search.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Show SOLIDWORKS search box | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSearchShowSOLIDWORKSSearchBox)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSearchShowSOLIDWORKSSearchBox, <OnFlag>) | Boolean value | Specifies whether to show the SOLIDWORKS search box |
| File and Model Search - Search while typing (incremental search) (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSearchWhileTyping) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSearchWhileTyping, <OnFlag>) | Boolean value | Specifies whether to start the search while typing the search string |
| File and Model Search - Include 3D ContentCentral results (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swSearchIncludeContentCentral) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swSearchIncludeContentCentral, <OnFlag>) | Boolean value | Specifies whether to start the search while typing the search string |
| File and Model Search - Results per page (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSearchResultsPerPage)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSearchResultsPerPage, <Value>) | Integer value | Specifies number of search results to show per page |
| File and Model Search - Maximum results per data source (independent of 3D ContentCentral) (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSearchMaxResultsPerDataSource)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSearchMaxResultsPerDataSource, <Value>) | Integer value | Specifies maximum number of results per data source (independent of 3D Content Central) |
| File and Model Search - Indexing Performance (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSearchIndexingPerformance)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swSearchIndexingPerformance, swSearchIndexingPerformance\_e.<Value>) | See swSearchIndexingPerformance\_e for valid options | Specifies when to perform search indexing |

Obsolete Enumerators

| Enumerator | Comment |
| swSearchDissectionScheduleDaily | Obsolete |
| swSearchDissectionDailyStartTime | Obsolete |
| swSearchDissectionDailyStopTime | Obsolete |
| swSearchDissectionLocation | Obsolete |