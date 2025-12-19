
Objective : perform a _persisted_ XSS attack with ``<iframe src="javascript:alert(`xss`)">`` without using the frontend application at all.

methodology : 

	Tools used :  Burp (Proxy,HTTP history,Repeater)

	1. The first step is to launch the site, search for the product and clik on.

	2. In the HTTP history, you will find a GET request with "/rest/product/../reviews" in the URL. Copy the entire content of this request.

	3. Paste the content into repeater. After a few tests, I found the correct url to use. Instead of "rest/product/../reviews" put "api/product/.." and send the request to get the product data and descriptiion.

	4.At the top of the request, replace GET with PUT. At the end, add "Content-Type: application/json", then skip a line and add the modified descripstion with the link you want in JSON format.