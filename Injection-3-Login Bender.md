methodology : 
	
	1-Access the login page.

	2-Identify the parameters sent during authentication.
	
	3-Inject a suitable SQL load into the login field.
	
	4-Analyze the server response.
	
	5-Validate access to the Bender account.
	
	Techniques used: SQL injection 
	Tools: Browser, Burp Suite

vulnerabilities :

	SQL Injection
	Poor management of SQL errors
	Severity: High
risks :

	Taking control of accounts
	Potential escalation to high privileges

actions :

	Prepared queries
	Secure error handling
	Logging of suspicious attempts