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
The web scanner can accept the following key value pair parameters:
lat - Latitude
long - Longtitude
gender - Gender (male/female/other)
dob - Date of Birth (YYYY-MM-DD per https://www.iso.org/iso-8601-date-and-time-format.html)
user-agent - User Agent of device
```objc
https://yourdomain.com/scan.html?lat=<latitude>&long=<longtitude>&gender=male&dob=2000-01-01&user-agent=<device user agent>
```
These are optional values and populating them will show up in the dashboard.


## Editing the intruction timer only applicable to scan2.html
User can edit the timer to show no result screen on timer to show up. note the unit is in milliseconds.
the default is 10000 milliseconds which is equal to 10 seconds.
```objc
//instruction timer
	options['instructionInterval'] = 10000;
```   

## Turning on geolocation
Users can choose whether to enable the geolocation setting on the web scanner. 
This would result in the web scanner prompting the user to allow location for the scanner.
Note if this option is turned off or the user rejects this permission, the dashboard will utilize the user's IP address to identify an approximate location.
```objc
	//set 0 to disable location
	options['geoloc'] = 1;
```   

Search using Image
----------------
Remember to put in the image and video triggers into the dashboard: [[https://dashboard.aiq.tech](https://dashboard.aiq.tech)) , else it would not return result.
![alt text](https://github.com/aiqtech/webscanner-html/blob/Image/dashboard.png)
Once done, you can start scanning! Happy scanning!


