# Example Usage

HTTP GET
<pre><code lang="">http://sms.rout2.com/hlr/api.php?msisdn=<b>MSISDN</b>&key=<b>KEY</b></code></pre>

cURL

``` bash
$ curl "http://sms.rout2.com/hlr/api.php?msisdn=MSISDN&key=KEY" 
```

PHP

``` php
<?php

$curl = curl_init();

curl_setopt_array($curl, array(
  CURLOPT_URL => "http://sms.rout2.com/hlr/api.php?msisdn=MSISDN&key=KEY",
  CURLOPT_RETURNTRANSFER => true,
  CURLOPT_ENCODING => "",
  CURLOPT_MAXREDIRS => 10,
  CURLOPT_TIMEOUT => 30,
  CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
  CURLOPT_CUSTOMREQUEST => "GET",
  CURLOPT_HTTPHEADER => array(
    "Cache-Control: no-cache",
  ),
));

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
  echo "cURL Error #:" . $err;
} else {
  echo $response;
}
```

Python

``` python
import requests

url = "http://sms.rout2.com/hlr/api.php"

querystring = {"msisdn":"MSISDN","key":"KEY"}

headers = {"Cache-Control": "no-cache"}

response = requests.request("GET", url, headers=headers, params=querystring)

print(response.text)
```

NodeJS

``` node
var request = require("request");

var options = { method: 'GET',
  url: 'http://sms.rout2.com/hlr/api.php',
  qs: { msisdn: 'MSISDN', key: 'KEY' },
  headers: { 'Cache-Control': 'no-cache' } };

request(options, function (error, response, body) {
  if (error) throw new Error(error);

  console.log(body);
});
```

C#
```c#
var client = new RestClient("http://sms.rout2.com/hlr/api.php?msisdn=MSISDN&key=KEY"); 
var request = new RestRequest(Method. GET); 
request. AddHeader("Cache-Control", "no-cache"); 
IRestResponse response = client. Execute(request); 
```

