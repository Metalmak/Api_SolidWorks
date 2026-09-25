<!-- source: sldworksapi/Set_Up_PropertyManager_Page_Slider_Control_Example_CPlusPlus_COM.htm -->

# SOLIDWORKS API Help

# Set Up PropertyManager Page Slider Control Example (C++ COM)

The following example shows how to set up a slider control.

...

id = CONTROL\_SLIDER;

controlType = swControlType\_Slider;

caption = \_T("");

alignment = swControlAlign\_Indent;

options = swControlOptions\_Visible + swControlOptions\_Enabled;

tip = \_T("Second trackbar");

hres = m\_pSwGroup\_1->IAddControl(id,
controlType, caption, alignment, options, tip, &m\_pSwControl\_1\_2);

if (m\_pSwControl\_1\_2 != NULL)

{

IPropertyManagerPageSlider\* pSlider = NULL;

HRESULT res = m\_pSwControl\_1\_2->QueryInterface(IID\_IPropertyManagerPageSlider,
(LPVOID\*)&pSlider);

if (pSlider != NULL)

{

res = pSlider->put\_Style(swPropMgrPageSliderStyle\_Vertical
| swPropMgrPageSliderStyle\_AutoTicks | swPropMgrPageSliderStyle\_BottomLeftTicks
| swPropMgrPageSliderStyle\_NotifyWhileTracking);

res = pSlider->SetRange(100,
200, &boolstatus);

res = pSlider->put\_Position(125);

res = pSlider->put\_LineSize(2);

res = pSlider->put\_PageSize(10);

res = pSlider->put\_Height(250);

pSlider->Release();

}

}

...