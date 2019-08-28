# webscanner-html
Easy Implementation of web scanner with HTML.

# scan.html and scan2.html
Users can pick between scan.html (User Interface which need clicking) or scan2.html (User interface with just scanning immidiately)

![alt text](https://github.com/aiqtech/webscanner-html/blob/Image/scan1.jpg)

&nbsp;  &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; <strong>scan.html</strong> &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp;  <strong>scan2.html</strong>



## Appid and appsecret 
Before using the aiq-wen-sdk, an AppID/Secret pair is required. 
This can be obtained from the client dashboard at: 
[[https://dashboard.aiq.tech](https://dashboard.aiq.tech))
You also need to ingest some image/video before you can search for them.

## Pairing with Webscanner
Once obtain you would need to enter the value got from the dashboard and key it into the web scanner.
```objc
  //replace with your app ID generated from your dashboard
	var appid = 'appid obtain from dashboard'; 
	//replace with your app secret generated from your dashboard
	var appsecret = 'appsecret obtained from dashboard';
``` 
## URL Parser
The function allows passing parameters like example date of birth and gender in the url, (All those parameters available in our API documentation: [[https://github.com/aiqtech/iq-Dashboard-Documents/blob/master/AIQ-Platform-Application-Rest-API.pdf](https://github.com/aiqtech/iq-Dashboard-Documents/blob/master/AIQ-Platform-Application-Rest-API.pdf))
```objc
  //replace with your app ID generated from your dashboard
var options = {};
	var searchParams = new URLSearchParams(window.location.search)
	searchParams.forEach(function(value, key) {
		options[key]=value;
	});
```  

## Editing the intruction timer only applicable to scan2.html
User can edit the timer to show no result screen on timer to show up. note the unit is in milliseconds.
the default is 10000 milliseconds which is equal to 10 seconds.
```objc
//instruction timer
	options['instructionInterval'] = 10000;
```   

## Turning on geolocation
Users can choose whether to pop up the enable the geolocation setting on the web scanner. 
Note if this option is turned off, the dashboard would not shown the location on the analytics.
```objc
//set 0 to disable location
	options['geoloc'] = 1;
```   

Search using Image
----------------
Remember to put in the image and video triggers into the dashboard: [[https://dashboard.aiq.tech](https://dashboard.aiq.tech)) , else it would not return result.
![alt text](https://github.com/aiqtech/webscanner-html/blob/Image/dashboard.png)
Once done, you can start scanning! Happy scanning!


