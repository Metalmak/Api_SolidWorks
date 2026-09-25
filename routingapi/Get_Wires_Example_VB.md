<!-- source: routingapi/Get_Wires_Example_VB.htm -->

# SOLIDWORKS Routing API Help

# Get Wires Example (VBA)

This example shows how to get the wires in a route.

...

Set rtElectricalRoute = rtRouteManager.GetElectricalRoute

...

lNumWiresAccumulated = 0

    vWires
= rtElectricalRoute.GetWires

    If
Not IsEmpty(vWires) Then

        lNumWires
= rtElectricalRoute.GetWiresCount

        ReDim
aWires(lNumWires - 1)

        lStartIdx
= lNumWiresAccumulated

        lEndIdx
= lNumWiresAccumulated + lNumWires - 1

        For
lIdx = lStartIdx To lEndIdx

            Set
aWires(lIdx) = vWires(lIdx)

            lNumWiresAccumulated
= lNumWiresAccumulated + 1

        Next
lIdx

    End
If

...