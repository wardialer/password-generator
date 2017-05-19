# password-generator
simple utility to generate secure random passwords on linux

## usage
```bash 
$ pwdgen [-l length] [-c charset]
```

## arguments
both arguments are optionals, defaults value are:
* LENGTH: 8
* CHARSET: graph

typical options for CHARSET parameter are:
* graph (all printable characters, not including space)
* alnum (all letters and digits)
* alpha (all letters)
* digit (all digits)

## examples
generating a 10 characters complex password:
```bash 
$ pwdgen -l 10
> L8#by77Hpo
```

generating a 8 characters alphanumeric password:

```bash 
$ pwdgen -l 8 -c alnum
> 0zxSLm4A
```
generating a 4 digits pin code:
```bash 
$ pwdgen -l 4 -c digit
> 6922
```
