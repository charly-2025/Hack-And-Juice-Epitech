methodology : 
	
	1-Perform a refund action.

	2-Intercept the request.
	
	3-Identify the financial parameters.
	
	4-Modify the values.
	
	5-Send the request.
	
	Techniques used: Abuse of business logic 
	Tools: Burp Suite
	
vulnerabilities :

	-Insufficient validation of business parameters
	-Lack of server control over critical values
	Severity: High
risks :

	-Financial manipulation
	-Fraud or illegitimate refund
	-Financial loss for the company

actions :

	-Server-side business validation