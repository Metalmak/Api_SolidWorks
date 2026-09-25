<!-- source: sldworksapiprogguide/Overview/PackedIntegersCPlusPlus.htm -->

# SOLIDWORKS API Help

# Unpacking Double Arrays into Integer Pairs in C++

Some API functions return integer information packed into arrays of
double values.

To extract the pair of integers from a double in C++, SOLIDWORKS suggests
using a union:

union PackedData\_

{

> double doubleValue;
>
> int intValues[2];

} PackedData;

int iValue1, iValue2;

To access the data, assign doubleValue
to the array element containing the data, then use
intValues to access the integers:

PackedData.doubleValue = dArray[0];

iValue1 = PackedData.intValues[0];

iValue2 = PackedData.intValues[1];