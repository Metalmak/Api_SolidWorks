<!-- source: sldworksapiprogguide/Overview/BOOL_and_VARIANT_BOOL_Are_Different_Types.htm -->

# SOLIDWORKS API Help

# BOOL and VARIANT\_BOOL Are Different Types

This topic describes:

* [BOOL and VARIANT\_BOOL differences](#BOOL)
* [S\_OK and S\_FALSE values](#S_OK)

## BOOL and VARIANT BOOL Differences

BOOL and VARIANT\_BOOL use different number values for TRUE:

## BOOL

* FALSE = 0
* TRUE  =
  1

## VARIANT\_BOOL

* VARIANT\_FALSE =  0
* VARIANT\_TRUE  =
  -1

However, many of the SOLIDWORKS COM APIs methods with VARIANT\_BOOL return
values return False or True (0 or 1). To ensure a correct comparison,
always compare the return value to 0. For example:

Dim bRetVal    As
Boolean

Dim lRetVal    As
Long

' Invoke method

bRetVal = swSomeObject.SomeMethod

' Inspect the numeric value

lRetVal = bRetVal

Debug.Print "Numeric value = & " lRetVal

' Inspect the logical value

If  (Not
(bRetVal = False)) Then   'If bRetVal Then will give incorrect
results

Debug.Print "Return value is True"

Else

Debug.Print "Return value is False"

End if

' Negate value

bRetVal = (bRetVal = False)   '
bRetVal = Not bRetVal will give
incorrect results

## S\_OK and S\_FALSE Values

The numeric values for S\_OK and S\_FALSE are:

* S\_OK = 0
* S\_FALSE = 1

These values should be type long in Visual Basic.