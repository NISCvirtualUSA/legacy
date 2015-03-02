# legacy
Legacy apps and widgets


##Instructions

###NGB Joint Information Exchange Environment - Events & Missions GeoRSS feed widget

For more information please visit http://www.jiee.info
credits: this widget was built using ESRI Flexviewer's GeoRSS widget.
Compiled for ArcGIS Flex Viewer v. 2.x

---------------------------------------------------------------------------------

####Installation instructions:

1. Copy the folders "JieeEventsWidget" and "JieeMissionsWidget" into the widgets folder of your Flex Viewer instance.
2. Add the following 2 tags to your Flex Viewer's config.xml file's <widgetcontainer> section
3. Update service URL for <SourceURL> tag in JieeEventsWidget.xml and/or JieeMissionsWidget to point to live service.

```
		<widget label="JIEE Events" left="50" top="50" preload="open"
		        icon="widgets/JieeEventsWidget/assets/images/jiee.png"
		        config="widgets/JieeEventsWidget/JieeEventsWidget.xml"
		        url="widgets/JieeEventsWidget/JieeEventsWidget.swf"/>
```
```
		<widget label="JIEE Missions" left="50" top="360" preload="open"
		        icon="widgets/JieeMissionsWidget/assets/images/jiee.png"
		        config="widgets/JieeMissionsWidget/JieeMissionsWidget.xml"
		        url="widgets/JieeMissionsWidget/JieeMissionsWidget.swf"/>
```


###KPI Editor widget

Credits: this widget was built using ESRI InfoTemplate widget.
Compiled for ArcGIS Flex Viewer v. 2.x

---------------------------------------------------------------------------------

####Installation instructions:

1. Copy the content of the KPI folder ("widgets", "popups", "assets") into your Flexviewer instance.
2. Add the following 2 tags to your Flex Viewer's config.xml file's <widgetcontainer> section
3. Update layer url parameter to your KPI Status service.
```
		 <layer label="OPS KPI Status" type="dynamic" visible="false" alpha="0.65"
               url="[enter KPI map service URL here]">
               <sublayer id="0" popupconfig="popups/PopUp_NEPilotOPS_Trans.xml"/>
               <sublayer id="1" popupconfig="popups/PopUp_NEPilotOPS_TransL.xml"/>
               <sublayer id="2" popupconfig="popups/PopUp_NEPilotOPS_PubHealth.xml"/>
               <sublayer id="3" popupconfig="popups/PopUp_NEPilotOPS_Power.xml"/>
               <sublayer id="4" popupconfig="popups/PopUp_NEPilotOPS_PowerArea.xml"/>
               <sublayer id="5" popupconfig="popups/PopUp_NEPilotOPS_CommsPT.xml"/>
               <sublayer id="6" popupconfig="popups/PopUp_NEPilotOPS_CommsArea.xml"/>
               <sublayer id="7" popupconfig="popups/PopUp_NEPilotOPS_KeyAssets.xml"/>
               <sublayer id="8" popupconfig="popups/PopUp_NEPilotOPS_Incident.xml"/>
               <sublayer id="9" popupconfig="popups/PopUp_NEPilotOPS_RSPT.xml"/>
               <sublayer id="10" popupconfig="popups/PopUp_NEPilotOPS_RSArea.xml"/>
         </layer> 
```