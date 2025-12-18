Objective : Change the `href` of the link within the [OWASP SSL Advanced Forensic Tool (O-Saft)](https://juice.cyber.epitest.eu/#/search?q=OWASP%20SSL%20Advanced%20Forensic%20Tool%20\(O-Saft\)) product description into  https://owasp.slack.com.

methodology : 

	Tools used :  Burp (Proxy,HTTP history,Repeater)

	1. The first step is to launch the site, search for the product and clik on.

	2. In the HTTP history, you will find a GET request with "/rest/product/../reviews" in the UR. Copy the entire content of this request.

	3. Paste the content into repeater. After a few tests, I found the correct url to use. Instead of "rest/product/../reviews" put "api/product/.." and send the request to get the product data and descriptiion.

	4.At the top of the request, replace GET with PUT. At the end, add "Content-Type: application/json", then skip a line and add the modified descripstion with the link you want.
	
vulnerabilities :

	Vulnerability type : Broken Access Control - Unauthorized Product Modification

	Affected components : 
		Product management API
		Porduct data in database

	Estimated severity : Critical
		Because attacket can change the product link with what they want

risks :

	Content manipulation : Attackers can change product data (description,price,...)

	Reputation damage : Modified product information reduces user trust in the platform

actions :

	Role Check : Ensure that you must be an admin to make sensitive request