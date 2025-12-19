methodology : 

	1-Access a feature protected by a CAPTCHA.

	2-Intercept the HTTP request with Burp Suite.
	
	3-Identify the parameter related to the CAPTCHA.
	
	4-Delete or change this setting.
	
	5-Send the modified request.
	
	6-Check that the action is accepted without CAPTCHA validation.
	
	Techniques used: Logical bypass 
	Tools: Burp Suite
vulnerabilities :

	CAPTCHA not verified server side
	Severity: Average
risks :

	Abusive automation
	Brute force attacks
actions :

	Systematically check the CAPTCHA on the server side
	Use dynamic tokens