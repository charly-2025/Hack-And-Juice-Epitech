
methodology : 

	Tools used : Burp (Proxy,HTTP history,Repeater)

	1. In the HTTP history, you will find a GET request with "search?q=" in the URL. Copy the entire content of this request

	2. Paste the content into repeater, on top,after the "search?q=" add a this "apple'))UNION%20SELECT%20sql,2,3,4,5,6,7,8,9%20FROM%20sqlite_master--", this SQL payload forces the database to return the SQL schema of all tables.

	3. Finaly, send the request.

vulnerabilities :

	Vulnerability type : SQL Injection - Union-based Injection
		
	Affected compnonent : 
		Search functionality
		SQL Database

	Estimated severity : Critical
		Because attackers can read database structure and prepare further attacks more efficiently

risks :

	Full database compromise : Attackers can retrieve database schema and prepare extraction of sensitive data

	Reputation damage : Exposure of customer internal data harm the platform's credibility

actions :

	Implement parameterized queries : Prepare the queries that will be made to the database


	Filter and validate user input : Only allow safe character for the search parameter