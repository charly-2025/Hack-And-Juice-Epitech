
Objective : Reset Jim's password via the Forgot Password mechanism with _the original answer_ to his security question.

methodology : 

	Tool used : OSINT

	1. The first step is to verify the security question, which is “Who is his older brother?”

	2. To begin my research, I need to know who Jim is. So I logged into Jim's account using an SQL injection to find information. In the saved addresses, I found an address that appeared to be in space.

	3. I did some more research on that address and on Jim, and I found information about James Tiberius Kirk in Star Trek.

	  4. Finally, by searching for “James Tiberius Kirk's older brother,” I found a name: Samuel, and it was the right name.

vulnerabilities :

	Vulnerability type : Broken Authentication – Weak Account Recovery Mechanism

	Affected compnonent : 
		Password recovery feature    
		Security question system

	Estimated severity : High
		Because attackers can reset user's password account and then get user's account 

risks :

	Account takeover : An attacker could reset the password of a user whose recovery answer is trivial or publicly known

	Loss of confidentiality : Unauthorized access to personal data, shopping history, or sensitive account information.

actions :

	Remove or harden security questions :  Avoid predictable questions
    
	Use secure password-reset feature : Sent by email link to reset password