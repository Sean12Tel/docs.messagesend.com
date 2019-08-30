# Home

## HLR Rest API


### Query String Values

| Name | Value |
|------|------------|
| MSISDN | The mobile number you wish to query. It should be written as E.164 format but without the + symbol. eg. Country code +44, with mobile number 07700 900123 should be written as 44700900123 |
| KEY | Your API Key |


### Example HTTP GET

<pre><code lang="">http://sms.rout2.com/hlr/api.php?msisdn=<b>MSISDN</b>&key=<b>KEY</b></code></pre>

### Response

``` json
{
  "result":{
    "msisdn":"447700900123",
    "imsi":"447700",
    "mcc":0,
    "mnc":0,
    "networkname":"T-mobile",
    "balance":"99.862",
    "errorCode":0
  }
}
```

