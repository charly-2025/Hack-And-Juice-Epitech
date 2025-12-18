
Objective : Log in with Chris' erased user account.

methodology : 

	1. The first step is to find Chris's email address. But that's easy, because most users have the same email address format, namely name@juice-sh.op. So Chris's email address is chris@juice-sh.op

	2. Logging in is even easier, as all you need to do is perform an SQL injection. To do this, on the login page in the email, simply add '-- at the end of the email.

	3. In password field, just enter any letter and you can login.
	
vulnerabilities :

	Vulnerability type : Broken Authentication - Improper Account Deletion
    
    Affected component :
	    User account management
        Database
    
    Estimated severity : High
		Because an erased account can still be accessed 

risks :

	Unauthorized access : An attacker can log in to accounts that should have been deleted.
	
	GDPR non-compliance : Personal data is not properly erased, exposing the organization to legal sanctions.

actions :

	Properly delete user accounts : Ensure deleted accounts are fully removed in the database.
