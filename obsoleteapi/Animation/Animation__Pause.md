<!-- source: obsoleteapi/Animation/Animation__Pause.htm -->

# Animation::Pause

This
method is:

* obsolete and has not been
  superseded.
* nonfunctional in SolidWorks
  2008 and later.

  Use the interfaces related to motion studies introduced in SolidWorks
  2008 to access animation and simulation.

Description

This method pauses the animation
at its current position.

Syntax (OLE Automation)

Retval = Animation.Pause ()

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) Retval | TRUE if the animation is paused at its current position, FALSE if the animation controller is not running |

#

Syntax (COM)

status = Animation->Pause ( &Retval)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) Retval | TRUE if the animation is paused and remains in its current position, FALSE if the animation controller is not running |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks