methodology : 
	tools used :  Burp
	
	-Analysis of the registration functionality
	-Interception of requests with Burp Suite
	-Observation of the parameters sent to the server
	-Test of modification of the values controlled by the user
	-Validation of server-side impact
	
vulnerabilities :

	-Insufficient validation of user inputs

	-Excessive trust in the data sent by the client

	-Lack of server verification of the user role

risks :

	-Unauthorized elevation of privileges

	-Access to administrator features

	-Complete compromise of the integrity of the application

actions :

	-Interception of the registration request via Burp Suite

	-Modification of the role parameter (role=admin)

	-Sending the modified request to the server

	-Successful creation of an account with administrator privileges