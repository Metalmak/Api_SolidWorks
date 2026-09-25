<!-- source: routingapi/GettingStarted-routingapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help |  |
| Getting Started |
| Send Feedback | |

Glossary Item Box

Writing a SOLIDWORKS Routing API application typically involves:

1. Adding a reference to SOLIDWORKS *version* Routing Type Library. Substitute the current SOLIDWORKS version number for *version*. For VBA and COM applications, add a reference to the type library, install\_dir\SWRoutingLib.tlb. For .NET applications, add a reference to the interop assembly, *install\_dir***\api\redist\SOLIDWORKS.interop.SWRoutingLib.dll**.

   - Instantiating a SOLIDWORKS connection.

     - Loading the SOLIDWORKS Routing add-in, if it is not already loaded, using the SOLIDWORKS ISldWorks::LoadAddIn method. The SOLIDWORKS Routing API DLL is sldrtadd.dll.

       - Opening a SOLIDWORKS assembly document that contains a route sub-assembly.

         - Using the SOLIDWORKS IAssemblyDoc::GetRouteManager method to get the SOLIDWORKS Routing API.

           - Getting the route.

             - Getting the cables and wires in the route.

               - Getting the route properties and editing the route.