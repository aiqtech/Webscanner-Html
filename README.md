# webscanner-html
Easy Implementation of web scanner with HTML.

# scan.html and scan2.html
Users can pick between scan.html (User Interface which need clicking) or scan2.html (User interface with just scanning immidiately)

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

Search using Image
----------------
Remember to put in the image and video triggers into the dashboard: [[https://dashboard.aiq.tech](https://dashboard.aiq.tech)) , else it would not return result.
Once done, you can start scanning! Happy scanning!

