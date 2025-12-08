
methodology : 

	Tools used : Burp (Proxy,HTTP history,Repeater)

	1. In the HTTP history, you will find a GET request with "search?q=" in the URL. Copy the entire content of this request

	2. Paste the content into repeater, on top,after the "search?q=" add a this "banana'))UNION%20SELECT%20sql,2,3,4,5,6,7,8,9%20FROM%20sqlite_master--", then send the request.

vulnerabilities :

risks :

actions :