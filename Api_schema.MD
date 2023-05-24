###### Acccess Bank PLC - 2023

#### Sample application interface documentation
```code
Documentation Version: 0.1.0
Version: 0.0.1
Author: Edilson Mucanze

Contributer:
    - OluwaTofarati Agbaje
    - Uchechukwu Obi
    - Oreoluwa Olayinka Abiodun
    - Edilson Mucanze
```

#### Group 10 - KSS
- This is a simple documentation schema for the sample APP in C#

**Glossary**
> API - Application Interface
> JSON - JavaScript Object Notation

___Base Endpoint___
http:/localhost:8080/api/v01/

### **API services**
- Accounts
- GetAccountByNbr
- GetAccountByClientNbr
- OpenAccount
- CheckOpenAccountStatus


#### [X] __Accounts__
This service will list customer accounts
```code
Endpoint: __BaseEndpoint__/Accounts
Method: POST
Accept: application/json
Authorization: Basic keypasstoken
```
```code
Request body - Not required
```
__Expected successful response__
```json
{
  "status_code": "000",
  "message": "Accounts List Retrieved.",
  "data" : [
    ....accountsObject,
    ....accountsObject
  ]
}
```

__Error response__
```json
{
  "status_code": "101",
  "message": "No Accounts yet.",
  "data": null,
  "error": {
    "message": "Error message",
    "code": "",
    "internal_info": ""
  }
}
```
