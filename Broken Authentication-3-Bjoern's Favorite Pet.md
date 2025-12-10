
methodology : 

	Tool used : Burp(Target), OSINT(Instagram)

	1. Go on Bjoern's Instagram and search the name of his favorite pet
	
	2. With Burp/Target go in rest/user/authentication-details you got 3 email

	3. Go in Forgot Pasword, the Email is bjoern@owasp.org and the security question awnser is Zaya

vulnerabilities :

	Vulnerability type : Broken Authentication – Weak Account Recovery Mechanism

	Affected compnonent : 
		Password recovery feature    
		Security question system

	Estimated severity : Critical
		Because attackers can reset user's password account and then get user's account 

risks :

	Account takeover : An attacker could reset the password of a user whose recovery answer is trivial or publicly known

	Loss of confidentiality : Unauthorized access to personal data, shopping history, or sensitive account information.

actions :

	Remove or harden security questions :  Avoid predictable questions
    
	Use secure password-reset feature : Sent by email link to reset password