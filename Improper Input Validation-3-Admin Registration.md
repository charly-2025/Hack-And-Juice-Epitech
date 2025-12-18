methodology : 

	1-Go to the registration page of the Juice Shop app.

	2-Fill in the form with valid information (email, password, etc.).

	3-Before submitting the form, intercept the HTTP request with Burp Suite.

	4-Analyze the parameters sent to the server.

	5-Identify a parameter related to the user role (e.g. role, isAdmin, userRole).

	6-Change the value of this setting to give it an administrator role.

	7-Send the modified request to the server.

	8-Verify that the account created has administrator privileges.

	Techniques used:
	-HTTP Interception
	-Parameter manipulation

	Tools:
	-Web browser
	-Burp Suite
	
vulnerabilities :

	Type: Improper Input Validation / Broken Access Control
	Affected component: Registration and role management system
	Cause: The server trusts the data sent by the client
	Estimated severity: High
risks :

	Creation of unauthorized administrator accounts
	Full access to sensitive features
	Total compromise of the application
	Loss of user trust

actions :

	Implement strict validation on the server side of user roles
	Never accept a role from a client request
	Define privileges only on the backend side
	Implement robust access controls