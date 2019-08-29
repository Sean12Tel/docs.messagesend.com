## Docs messagesend.com

Example Usage

HTTP GET
```
http://sms.rout2.com/hlr/api.php?msisdn=MSISDN&key=KEY
```

cURL
```bash
$ curl "http://sms.rout2.com/hlr/api.php?msisdn=MSISDN&key=KEY" 
```

PHP
```php
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
