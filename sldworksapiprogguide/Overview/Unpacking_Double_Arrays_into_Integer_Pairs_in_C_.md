<!-- source: sldworksapiprogguide/Overview/Unpacking_Double_Arrays_into_Integer_Pairs_in_C_.htm -->

# SOLIDWORKS API Help

# Unpacking and Packing Arrays in C#

Some of the arguments passed from and to SOLIDWORKS using the API
contain arrays of doubles. In some functions, elements in these arrays
contain two integers packed into a double array element. You can unpack
the data from a double to two integers and vice versa.

using System;

using System.Runtime.InteropServices;

namespace WindowsApplication2

{

[StructLayout(LayoutKind.Explicit)]

public struct DoubleIntConv

{

// An 8-byte double contains 2 4-byte ints.

[FieldOffset(0)] private int    m\_Int1;

[FieldOffset(4)] private int    m\_Int2;

[FieldOffset(0)] private double m\_Double;

private DoubleIntConv(double dValue)

{

//C# wants these initialized in the constructor

m\_Int1 = 0; m\_Int2 = 0;

m\_Double = dValue;

}

private DoubleIntConv(int iValue1, int iValue2)

{

//C# wants this initialized in the constructor

m\_Double = 0.0;

m\_Int1 = iValue1; m\_Int2 = iValue2;

}

//Use out
parameters, so client code can pass in an uninitialized variable

//Unpack

public static void Unpack (double dIn, out
int iOut1, out int iOut2)

{

DoubleIntConv   cv;

cv = new DoubleIntConv(dIn);

iOut1 = cv.m\_Int1;

iOut2 = cv.m\_Int2;

return;

}

//Use an out parameter, so client code
can pass in an uninitialized variable

//Pack

public static void Pack (int iIn1, int iIn2,
out double dOut)

{

DoubleIntConv   cv;

cv = new DoubleIntConv(iIn1, iIn2);

dOut = cv.m\_Double;

return;

}

      class Program

      {

  [STAThread]

  static void Main()

  {

int             iValueIn1
 = 65535;

int             iValueIn2
 = 0;

double          dValueOut;

int             iValueOut1;

int             iValueOut2;

DoubleIntConv.Pack(iValueIn1, iValueIn2,
out dValueOut);

DoubleIntConv.Unpack(dValueOut, out iValueOut1,
out iValueOut2);

return;

  }

      }

}

See
Create
Reference Curve Example (C#) for an example of packing an array.