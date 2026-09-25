<!-- source: obsoleteapi/Animation/Animation__End.htm -->

# Animation::End

This
method is:

* obsolete and has not been
  superseded.
* nonfunctional in SolidWorks
  2008 and later.

  Use the interfaces related to motion studies introduced in SolidWorks
  2008 to access animation and simulation.

Description

This method positions the
animation at its ends.

Syntax (OLE Automation)

Retval = Animation.End ()

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) Retval | TRUE if the animation is positioned at its ends, FALSE if the animation controller is not running |

#

Syntax (COM)

status = Animation->End ( &Retval)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) Retval | TRUE if the animation is positioned at its ends, FALSE if the animation controller is not running |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks