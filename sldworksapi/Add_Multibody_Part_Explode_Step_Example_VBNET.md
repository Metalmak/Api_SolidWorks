<!-- source: sldworksapi/Add_Multibody_Part_Explode_Step_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Add Multibody Part Explode Step Example (VB.NET)

This example shows how to create an explode view of a multibody part.

'-----------------------------------------------------------------------------

'
Preconditions:

' 1. Open
*public\_documents***\samples\tutorial\multibody\multi\_Inter.sldprt**.

' 2. Open
an Immediate window.

'

'
Postconditions:

' 1.
Creates **Exploded View1** in ConfigurationManager.

' 2. Adds
**Chain1** to **Exploded View1**.

' 3.
Displays the **Exploded View1** in its exploded state.

' 4.
Inspect the Immediate window, the ConfigurationManager,

'

and the graphics area.

'

' Note:
Because the model is used elsewhere, do not save any changes.

'----------------------------------------------------------------------------

Imports SolidWorks.Interop.sldworks

Imports SolidWorks.Interop.swconst

Imports System.Runtime.InteropServices

Imports System

Partial
Class
SolidWorksMacro

Sub main()

Dim swModel
As
PartDoc

Dim config
As
Configuration

Dim configName
As
String

Dim swMdl
As
ModelDoc2

Dim explStep
As
PartExplodeStep

Dim comp
As
Body2

Dim var
As
Object

Dim varViews
As
Object

Dim configVar
As
Object

Dim boolstatus
As
Boolean

Dim i
As
Long

Dim errCode
As
Long

swModel = swApp.ActiveDoc

swMdl = swModel

configVar = swMdl.GetConfigurationNames

Call swModel.**CreateExplodedView**

varViews = swModel.**GetExplodedViewNames**(configVar(0))

configName = swModel.**GetExplodedViewConfigurationName**(varViews(0))

config = swMdl.GetConfigurationByName(configName)

swModel.**ShowExploded**(True, varViews(0))

        'Select the bodies to move

boolstatus = swMdl.Extension.SelectByID2("Extrude-Thin1",
"SOLIDBODY", 0, 0, 0,
True, 1,
Nothing, 0)

'Add an explode
step without selecting an explode direction entity

'Defaults to the
Z-direction manipulator index

explStep = config.**AddPartExplodeStep**("Exploded View1", 0.07, -1,
False,
True, errCode)

Call swMdl.EditRebuild3

'Get bodies
moved in the explode step

var = explStep.**GetBodies**()

Debug.Print("Explode view: " & varViews(0))

Debug.Print("Explode step: " & explStep.**Name**)

Debug.Print("Explode distance (m): " & explStep.**ExplodeDistance**)

Debug.Print("Reverse translation direction? " &
explStep.**ReverseTranslationDirection**)

Debug.Print("Automatically space components on
drag? " & explStep.**AutoSpaceBodiesOnDrag**)

Debug.Print("Bodies moved in the explode step:")

For i = 0
To UBound(var)

comp = var(i)

Debug.Print("

" & comp.Name)

Next

End
Sub

'''
<summary>

''' The SldWorks swApp variable is pre-assigned for you.

'''
</summary>

Public swApp
As
SldWorks

End
Class