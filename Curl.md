# curl command notes
### Difinition :
`curl (short for "Client URL") is a command line tool that enables data transfer over various network protocols. It communicates with a web or application server by specifying a relevant URL and the data that need to be sent or received`

### Usages : 
- Downloading files from the internet
- Endpoint testing
- Debugging
- Error logging


### General Syntax :
> curl  \[flags] \[url]

### HTTP METHODS :
> curl -X \[METHOD] \[URL] // default : GET

##### Examples :
```
curl -X POST https://www.target.com
curl -X PUT https://www.target.com
curl -X TRACE https://www.target.com
curl -X DELETE https://www.target.com
curl -X OPTIONS https://www.target.com
```
### SEND DATA :

> curl -X POST -d "name=ahmed&age=21" https://jsonplaceholder.typicode.com/users // d : data

> curl -X POST -d '{"name":"ahmed","age":"12"}' -H "Content-Type:application/json" https://jsonplaceholder.typicode.com/users 

### DOWNLOADING images AND files :
> curl <file-link> -o filename.extension

##### Examples :
> curl https://staticg.sportskeeda.com/editor/2022/05/db755-16523472655799-1920.jpg -o kill.jpg
  
## For more Information :
> Visit [docs](https://phoenixnap.com/kb/curl-command)












