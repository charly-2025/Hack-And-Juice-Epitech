methodology : 

	1-Access the upload form.

	2-Select an unauthorized file.
	
	3-Intercept the request.
	
	4-Edit the Content-Type or extension.
	
	5-Send the request.
	
	Techniques used: Filter bypass 
	Tools: Burp Suite

vulnerabilities :

	Insufficient type validation
	Severity: High
risks :

	Upload malicious files
	Execution of arbitrary code
	Server compromise

actions :

	Strict server validation
	Whitelist of allowed types