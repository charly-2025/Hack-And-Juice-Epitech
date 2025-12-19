
Objective : Retrieve a list of all user credentials via SQL Injection.

methodology : 

	Tools used : Burp (Proxy,HTTP history,Repeater)

	1. In the HTTP history, you will find a GET request with "search?q=" in the URL. Copy the entire content of this request

	2. Paste the content into repeater, on top,after the "search?q=" add a this "apple'))UNION%20SELECT%20email,password,3,4,5,6,7,8,9%20FROM%20Users--", this SQL payload forces the database to return all Users Data

	3. Finaly, send the request. UNION is used to add another SQL query, 20% is used to add space. For UNION, it is important to have the same number of columns returned

vulnerabilities:

    Vulnerability type : SQL Injection – UNION-based Injection

    Affected component :
        Search feature
        Backend database
        Users table

    Estimated severity : Critical
        Because attackers can retrieve all user credentials including emails and passwords

risks:

    Data breach : Leakage of all user credentials stored in the database

    Account takeover : Stolen credentials can be reused to access user accounts

actions:

	Implement parameterized queries : Prepare the queries that will be made to the database

	Filter and validate user input : Only allow safe character for the search parameter


