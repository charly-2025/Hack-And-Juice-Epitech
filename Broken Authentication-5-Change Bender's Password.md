
Objective : Change Bender's password into _slurmCl4ssic_ without using SQL Injection or Forgot Password.

methodology : 

	Tool used : Burp(HTTP History, Repeater)

	1. First step is to login at the Bender's account because we will use the password change mechanism 

	2. Once your are on the password change page you should attemps to change password with a random Current password and enter slurmCl4ssic in New and Repeat Password fields

	3. In HTTP History, find the request with "change password" in URL and copy the content

	4. Paste it into Repeater and just remove all about current password at the top of request, and send the request

vulnerabilities :

	Vulnerability type : Broken Authentication – Missing Verification of Current Password

	Affected component :
		 Password change mechanism
	    User account
    
	Estimated severity : Critiacl  
	Because an attacker can change a user’s password without knowing the current one

risks :

	Account takeover : An attacker can change the victim’s password and lock them out of their account.
	
	Loss of confidentiality : Unauthorized access to personal data and account information.

actions :

	Enforce current password verification : The server must always validate the current password before allowing a password change.
