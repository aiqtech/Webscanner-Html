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
## Pairing with Webscanner
Once obtain you would need to enter the value got from the dashboard and key it into the web scanner.
```objc
//instruction timer
	options['instructionInterval'] = 10000;
```   

Search using Image
----------------
Remember to put in the image and video triggers into the dashboard: [[https://dashboard.aiq.tech](https://dashboard.aiq.tech)) , else it would not return result.
![alt text](https://github.com/aiqtech/webscanner-html/blob/master/Screen%20Shot%202019-08-27%20at%2012.20.31%20PM.png)
Once done, you can start scanning! Happy scanning!


