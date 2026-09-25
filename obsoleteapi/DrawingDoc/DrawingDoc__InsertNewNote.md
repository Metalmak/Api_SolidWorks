<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__InsertNewNote.htm -->

# DrawingDoc::InsertNewNote

This method is obsolete and has been superseded
by DrawingDoc::InsertNewNote2.

Description

This method creates a new note in this drawing.

Syntax (OLE Automation)

void DrawingDoc.InsertNewNote ( text,
noLeader, balloonNote, bentLeader, arrowStyle, leaderSide)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) text | Text string to be put in the note |
| Input: | (BOOL) noLeader | TRUE does not add a leader line, FALSE does |
| Input: | (BOOL) balloonNote | TRUE adds balloon, FALSE does not |
| Input: | (BOOL) bentLeader | TRUE adds a bent leader line, FALSE does not |
| Input: | (short) arrowStyle | Arrowhead type as defined in swArrowStyle\_e |
| Input: | (short) leaderSide | Leader line side as defined in swLeaderSide\_e |

Syntax (COM)

status = DrawingDoc->InsertNewNote
( text, noLeader, balloonNote, bentLeader, arrowStyle, leaderSide )

| Input: | (BSTR) text | Text string to be put in the note |
| Input: | (VARIANT\_BOOL) noLeader | TRUE does not add a leader line, FALSE does |
| Input: | (VARIANT\_BOOL) balloonNote | TRUE adds a balloon, FALSE does not |
| Input: | (VARIANT\_BOOL) bentLeader | TRUE adds a bent leader line, FALSE does not |
| Input: | (short) arrowStyle | Arrowhead type as defined in swArrowStyle\_e |
| Input: | (short) leaderSide | Leader line side as defined in swLeaderSide\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks