methodology : 
	
	1-Identify a parameter subject to validation.

	2-Add a null byte character (%00) in the value.
	
	3-Send the request.
	
	4-Observe the validation bypass.
	
	Techniques used: Special character injection 
	Tools: Burp Suite

vulnerabilities :

	Poor management of null characters
	Severity: Average

risks :

	Bypass of security controls
	Unauthorized access to resources

actions :

	Strict cleaning of the entrances
	Robust server validation