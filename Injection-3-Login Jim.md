methodology : 

	1-Access the Juice Shop login page.

	2-Identify the fields used for authentication (email / password).

	3-Test the application’s behavior in the face of abnormal inputs.

	4-Inject a simple SQL load into the email or password field.

	5-Observe the server’s response.

	6-Adjust the load until getting a bypass of authentication.

	7-Check access to user Jim’s account.

	Techniques used: SQL injection 
	Tools: Browser, Burp Suite

vulnerabilities :

	SQL Injection
	Absence of prepared queries	
	Insufficient filtering of user inputs
	Severity: High
risks :

	Unauthorized access to user accounts
	Personal data leak
	Compromise of the authentication system
	 
actions :

	Use prepared statements
	Escape and validate all user inputs
	Implement injection detection mechanisms