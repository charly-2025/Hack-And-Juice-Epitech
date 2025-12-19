Objective: exploit a compromised external dependency used by the application.

Methodology :

	1-Analyze the application features relying on external libraries.
	
	2-Identify a feature using a third-party component (e.g. JavaScript dependency).
	
	3-Look for clues that the loaded library is unreliable or has been modified.
	
	4-Observe the abnormal behavior of the application related to this component.
	
	5-Exploit the vulnerability introduced by the compromised dependency.
	
	6-Validate the success of the challenge via the success indicator.
	
	Techniques used:
	Dependency analysis
	Supply chain operation
Vulnerabilities:

	Type: 
	Vulnerable and Outdated Components / Supply Chain Attack
	
	Component affected: 
	Third-party library integrated into the application
	
	Cause: 
	External dependency compromised or unverified
	
	Estimated severity: Criticism

Risks:

	Execution of malicious code on the client or server side
	Complete compromise of the application
	Damage to the company’s reputation

Actions:

	Check the integrity of dependencies (hash, signature)
	Host critical libraries locally
	Implement a dependency management policy
	Regularly update third-party components