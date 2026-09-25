<!-- source: obsoleteapi/Animation/Animation__Beginning.htm -->

# Animation::Beginning

This method is:

* obsolete and has not been
  superseded.
* nonfunctional in SolidWorks
  2008 and later.

  Use the interfaces related to motion studies introduced in SolidWorks
  2008 to access animation and simulation.

Description

This method positions the
animation at its beginning.

Syntax (OLE Automation)

Retval = Animation.Beginning ()

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) Retval | TRUE if the animation is positioned at its beginning, FALSE if an animation controller is not running |

#

Syntax (COM)

status = Animation->Beginning ( &Retval)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) Retval | TRUE if the animation is positioned at its beginning, FALSE if an animation controller is not running |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks