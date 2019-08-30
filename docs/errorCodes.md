# Error Codes

### Error Code Table
| Code | Descrition |
|------|------------|
|0|Success|
|1|Authentication Failure. Check Key|
|2|Not Enough Balance|
|3|MSISDN Not Valid|
|4|HLR Lookup not configured for prefix|
|5|Uknown Network Error|
|6|Network Error. Check Error Description for more info|
|7|API Data Mismatch Error|

### Example Error Response
```json
{
    "result":{
        "error":"key not valid",
        "errorCode":1
    }
}
```