<!-- source: cworksapi/GettingStarted-swsimulationapi.html -->

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
| SOLIDWORKS Simulation API Help |  |
| Getting Started |
| Send Feedback | |

Glossary Item Box

Writing a SOLIDWORKS Simulation application typically involves:

1. Instantiating a SOLIDWORKS connection.

   - Accessing the SOLIDWORKS Simulation add-in object. Read Accessing SOLIDWORKS Add-in Objects.

     - Getting the [COSMOSWorks](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICosmosWorks.html) object.

       - Getting the [model document](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWModelDoc.html) object. Opening a document is required before trying to create a study.

         - Using the [study manager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyManager.html) object to create a study.

           - After creating a study, you can use the SOLIDWORKS Simulation API to:

             * define materials

               * apply loads and restraints relevant to the study

                 * apply contact features

                   * apply mesh control

                     * mesh the model

                       * run the study

                         * process the results

#### Error Handling

When appropriate, the Simulation API returns an error status code. Sometimes, directly returning a status code is not possible. When appropriate, the SOLIDWORKS Simulation API returns an error code (a 32-bit value) which is 0 for success and non-0 for error.

SOLIDWORKS Simulation recommends that you use the intrinsic Visual Basic Err object to get rich error information. In this case, the Err.number field does not correspond directly to the SOLIDWORKS Simulation error code, but mappings back to the error code are provided. The Err.Description field contains a descriptive text field indicating the error. Better tracing of errors can be done through the Err object.

In Visual Basic, error handling can easily be accomplished with the On Error Resume Next statement.

#### pidcollector.exe

An executable (**pidcollector.exe**) is provided in *install\_dir***\api** to help you get the persistent IDs of selected entities.

To use pidcollector.exe:

1. Double-click **pidcollector.exe** while SOLIDWORKS is running and a SOLIDWORKS document is active.- Make a selection in the document and click **Copy PIDS to clipboard** in the PID Collector dialog.- Paste the text copied to the clipboard into your application.- Edit the pasted text as needed.- Repeat steps 2 through 4 for each selection for which you want its PID.