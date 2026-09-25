<!-- source: obsoleteapi/SplitBodyFeatureData/SplitBodyFeatureData__State.htm -->

# SplitBodyFeatureData::State

This property is obsolete and has been superseded
by SpitBodyFeatureData::Consume.

Description

This property gets the
state of the resultant bodies of this split-body feature.

Syntax (OLE Automation)

\*state = SplitBodyFeatureData.State
(VB Get property)

SplitBodyFeatureData.State = state
(VB Set property)

\*state = SplitBodyFeatureData.GetState ( ) (C++ Get
property)

SplitBodyFeatureData.SetState ( state
) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Output: | (long ) \*state | State as defined in swSplitBodyType\_e |

#

Syntax (COM)

status = SplitBodyFeatureData->get\_State
( &state )

status = SplitBodyFeatureData->put\_State
( state )

|  |  |  |
| --- | --- | --- |
| Output: | (long ) \*state | State as defined in swSplitBodyType\_e |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks