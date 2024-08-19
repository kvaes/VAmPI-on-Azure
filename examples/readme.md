### Example
Install the rest client extension in VS Code (https://marketplace.visualstudio.com/items?itemName=humao.rest-client) , and use the users.http script.
More background info can be found here ; https://blog.held.codes/vampi-vulnerable-api-write-up-and-walk-through-3cce519e5e96
Also check api_vies/users.py & models/user_model.py

### SQL Injection test
Install sqlmap & wafw00f, and then execute the statements in kali.cli
This allows you to test vulnerable code when exposed directly, or via a WAF. And what the result would be with the alternative secured code.