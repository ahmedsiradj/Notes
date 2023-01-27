#Insecure Direct Object References :
**IDOR happen whene users can `access resources that do not belong to them` by directly reference the object `ID`,`Object Number`,`filename` ...etc**

## Hunting for IDOR :
* Source code review
* Capture requests for `parameters`,`numbers`,`username` ...etc 
* If the application is using **hashed** or **randomized** IDs try to `decode` it or `predict` it 
* Change the http requests `POST`,`HEAD`,`PUT`,`DELETE` ... etc
* Change the requested `filetype`\(extentions)
* Pay attention to features that return `sensitive information`

## How to prevent IDOR's :
* Check the user's identity and permissions \(`sissions-key`,`cookies`,`tokens` ...etc)
* Use **unique**, **unpredictable key** \(i.e: `.../profile?user-key=Gf98z...`)
