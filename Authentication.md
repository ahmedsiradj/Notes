# Authentication Testing :

* change login page protocols from `HTTPS` to `HTTP` \(remove `S`, i.e:http://www.example.org/login).
* The interactions to test include the following:
  - Forms that allow users to handle forgotten password or other credential,edit credentials.
  - Forms that require the user to authenticate with another provider (for example, payment processing).
* Testing for Default Credentials \(i.e:`admin`, `administrator`, `root`, `system`, `guest`, `operator`, or `super`).
* Capture every requests for finding `hidden parameters`, interesting GET request `(login=yes)`, ...etc .
* Look for  `source code comments` for intersting data .
* look in backup directories or backups of source code .
* Attempt to log in with an incorrect password 3 times or more ...,and \(capture error message).
* Review if the application stores sensitive information on the client-side.
* Review if access can occur without authorization.
* Check to not send the parameters \(do not send any or only 1).
* Change content type to json \("Content-Type:application/json") and send `json values`.
* If you get a response saying that POST is not supported you can try to send the JSON in the body but with a GET request with `Content-Type: application/json`.
* If you can send a JSON object you can send `"password":{"password": 1}` to bypass the login.
