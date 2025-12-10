c
methodology : 

	Tools used :  Burp (Proxy,HTTP history,Repeater)

	1. The first step is to launch the site, write go to the http history on Burp, and then add a product to your basket.

	2. In the HTTP history, you will find a POST request with BasketId in the URL. Copy the entire content of this request.

	3. Paste the content into repeater, add a second basketId (the one belonging to the person you want to add a product to) below the first one, then send the request.
	
vulnerabilities :

	Vulnerability type : Broken Access Control - Insercure Direct Object Reference
	
	Affected compnonent : 
		Basket mangement update API
		Database storing basket contents

	Estimated severity : Critical
		Because attackers can interfere with customer's shopping basket
	
risks :

	Data integrity compromise : Basket content can be altered 

	Financial impact : Unauthorized modifications may cause unexpected purchases

	Loss of customer trust : Users may lose confidence in the platform

actions :

