## Full Reset Password Journey

### 1. Issue Token

endpoint:

```text
GET https://gateway.zeepay.com.tr/v2/Authorization/IssuingToken
```

Headers:

```json
{
  "TenantId": "50e82747-9534-11f0-875f-06e024ab308d",
  "Token": "50e83c46-9534-11f0-875f-06e024ab308d"
}
```

Payload:

```json
{}
```

Response:

```json
{
  "result": {
    "code": 200,
    "status": "Success"
  },
  "response": {
    "token": {
      "access": "NWlYM2pkYkxiTnBINEZkSEpJQkRvTE9SeHVDbE5VdEZWTFJuNnlORXUwL2JRWk9Qd1BrRldnbnp3a05XcUJFUVltV0RyV0YyK05PVXZHT290WlZyNTAwUm95bDl4Qk5VUnBQV2JFZzN4VG5uMzRFVEZFSnVLVTV3cVJHM0x1MmNnU2JTZWFCL2NPbEV3MjhUd3l0UytQa2wwellsRWJPMjRJUWN6bXJOc1JvRmdGMXJkMWpkczNVeWJTbGR1L3RRZGFRU3ZiRFZWWEkvaDBhTEN3YTA2aUVXUTVsSUxyZlczN21ZOWcxMGNrczl4NS9ybWg0ei8rWThvTDo6j+p06EMmHyn8Ft1X8l3Biw==.500485f35a5ec73eac7ed504e52f2df5684cb10dbb5795b93c4ce57c29a38f80.N0RXaVRtcmRValA1eGtObDdQalQzbHpCK0cra0xJVzFmN25XaGJvRmlCWW9tdlV0TFRybEtIZ3hvTE15Q3FaVmdqaS9yVzRCVDd0YVNycHIzcG1iSlRzMHNLTW0wZldQL2tmd3VPK1k4cVRpYzNrRDJXTnFsbTY5QmV0YzAvQXlUOFpXNTM2RHhlQnljb0FsNTlVenE2OE5SdjFONGVuOCtsRUQyUE55NUs4UkQrTXN3V3kvYkYvdjRFaWxWYVlYa1ZIdGp0MXZyLytIYXhtU1lRVm51T2VFcWNuV04wcDJZTlpNMERjT3NHcDYyRmNvcHpYWnpZSGVlM2RsWUxTRk0xWnhUcFEzdTFOelJS",
      "expires": "2026-05-19T00:47:34.593516Z",
      "timezone": "UTC",
      "type": "Bearer"
    }
  }
}
```

### 2. Reset Password By Phone Number

endpoint:

```text
POST https://gateway.zeepay.com.tr/v2/Customer/ResetPassword/ResetPasswordByPhoneNumber
```

Headers:

```json
{
  "Authorization": "NWlYM2pkYkxiTnBINEZkSEpJQkRvTE9SeHVDbE5VdEZWTFJuNnlORXUwL2JRWk9Qd1BrRldnbnp3a05XcUJFUVltV0RyV0YyK05PVXZHT290WlZyNTAwUm95bDl4Qk5VUnBQV2JFZzN4VG5uMzRFVEZFSnVLVTV3cVJHM0x1MmNnU2JTZWFCL2NPbEV3MjhUd3l0UytQa2wwellsRWJPMjRJUWN6bXJOc1JvRmdGMXJkMWpkczNVeWJTbGR1L3RRZGFRU3ZiRFZWWEkvaDBhTEN3YTA2aUVXUTVsSUxyZlczN21ZOWcxMGNrczl4NS9ybWg0ei8rWThvTDo6j+p06EMmHyn8Ft1X8l3Biw==.500485f35a5ec73eac7ed504e52f2df5684cb10dbb5795b93c4ce57c29a38f80.N0RXaVRtcmRValA1eGtObDdQalQzbHpCK0cra0xJVzFmN25XaGJvRmlCWW9tdlV0TFRybEtIZ3hvTE15Q3FaVmdqaS9yVzRCVDd0YVNycHIzcG1iSlRzMHNLTW0wZldQL2tmd3VPK1k4cVRpYzNrRDJXTnFsbTY5QmV0YzAvQXlUOFpXNTM2RHhlQnljb0FsNTlVenE2OE5SdjFONGVuOCtsRUQyUE55NUs4UkQrTXN3V3kvYkYvdjRFaWxWYVlYa1ZIdGp0MXZyLytIYXhtU1lRVm51T2VFcWNuV04wcDJZTlpNMERjT3NHcDYyRmNvcHpYWnpZSGVlM2RsWUxTRk0xWnhUcFEzdTFOelJS",
  "Content-Type": "application/json"
}
```

Payload:

```json
{
  "id": "01f1562b7-5a92-ae60-ad7a-0809548288d2",
  "captcha": "bzhqn",
  "phone_country_code": "98",
  "phone_number": "9125264665",
  "customer_ip": "93.115.127.129"
}
```

Response:

```json
{
  "result": {
    "code": 200,
    "status": "Success",
    "request_number": "1779108454.769703.753557"
  },
  "response": {
    "sms": {
      "receiver": "+98*******665",
      "reference": "01f1562b7-be2a-3c20-985c-a6f2c35cfc4f",
      "expires": "2026-05-18T12:50:34.778126Z",
      "timezone": "UTC"
    }
  }
}
```

### 3. Authenticate OTP

endpoint:

```text
POST https://gateway.zeepay.com.tr/v2/Customer/Authentication/Authentication
```

Headers:

```json
{
  "Authorization": "NWlYM2pkYkxiTnBINEZkSEpJQkRvTE9SeHVDbE5VdEZWTFJuNnlORXUwL2JRWk9Qd1BrRldnbnp3a05XcUJFUVltV0RyV0YyK05PVXZHT290WlZyNTAwUm95bDl4Qk5VUnBQV2JFZzN4VG5uMzRFVEZFSnVLVTV3cVJHM0x1MmNnU2JTZWFCL2NPbEV3MjhUd3l0UytQa2wwellsRWJPMjRJUWN6bXJOc1JvRmdGMXJkMWpkczNVeWJTbGR1L3RRZGFRU3ZiRFZWWEkvaDBhTEN3YTA2aUVXUTVsSUxyZlczN21ZOWcxMGNrczl4NS9ybWg0ei8rWThvTDo6j+p06EMmHyn8Ft1X8l3Biw==.500485f35a5ec73eac7ed504e52f2df5684cb10dbb5795b93c4ce57c29a38f80.N0RXaVRtcmRValA1eGtObDdQalQzbHpCK0cra0xJVzFmN25XaGJvRmlCWW9tdlV0TFRybEtIZ3hvTE15Q3FaVmdqaS9yVzRCVDd0YVNycHIzcG1iSlRzMHNLTW0wZldQL2tmd3VPK1k4cVRpYzNrRDJXTnFsbTY5QmV0YzAvQXlUOFpXNTM2RHhlQnljb0FsNTlVenE2OE5SdjFONGVuOCtsRUQyUE55NUs4UkQrTXN3V3kvYkYvdjRFaWxWYVlYa1ZIdGp0MXZyLytIYXhtU1lRVm51T2VFcWNuV04wcDJZTlpNMERjT3NHcDYyRmNvcHpYWnpZSGVlM2RsWUxTRk0xWnhUcFEzdTFOelJS",
  "Content-Type": "application/json"
}
```

Payload:

```json
{
  "receiver": "+989125264665",
  "code": "463219",
  "reference": "01f1562b7-be2a-3c20-985c-a6f2c35cfc4f",
  "customer_ip": "93.115.127.129"
}
```

Response:

```json
{
  "result": {
    "code": 200,
    "status": "Success",
    "request_number": "1779108525.173947.151458"
  },
  "response": {
    "unique_id": "f9e538b255c06209475e13d3f792cd0a14365c8ce417a9bef079762e9dfe0d60",
    "customer_key": "c0115490a57e0423165df3803ae2f106",
    "packed": "I-*PHOdwlYFNwsR9eH62dJyy&Z",
    "active_datetime": "2026-05-18T12:51:45.192179Z",
    "timezone": "UTC"
  }
}
```

### 4. Set New Password

endpoint:

```text
POST https://gateway.zeepay.com.tr/v2/Customer/ResetPassword/SetPassword
```

Headers:

```json
{
  "Authorization": "NWlYM2pkYkxiTnBINEZkSEpJQkRvTE9SeHVDbE5VdEZWTFJuNnlORXUwL2JRWk9Qd1BrRldnbnp3a05XcUJFUVltV0RyV0YyK05PVXZHT290WlZyNTAwUm95bDl4Qk5VUnBQV2JFZzN4VG5uMzRFVEZFSnVLVTV3cVJHM0x1MmNnU2JTZWFCL2NPbEV3MjhUd3l0UytQa2wwellsRWJPMjRJUWN6bXJOc1JvRmdGMXJkMWpkczNVeWJTbGR1L3RRZGFRU3ZiRFZWWEkvaDBhTEN3YTA2aUVXUTVsSUxyZlczN21ZOWcxMGNrczl4NS9ybWg0ei8rWThvTDo6j+p06EMmHyn8Ft1X8l3Biw==.500485f35a5ec73eac7ed504e52f2df5684cb10dbb5795b93c4ce57c29a38f80.N0RXaVRtcmRValA1eGtObDdQalQzbHpCK0cra0xJVzFmN25XaGJvRmlCWW9tdlV0TFRybEtIZ3hvTE15Q3FaVmdqaS9yVzRCVDd0YVNycHIzcG1iSlRzMHNLTW0wZldQL2tmd3VPK1k4cVRpYzNrRDJXTnFsbTY5QmV0YzAvQXlUOFpXNTM2RHhlQnljb0FsNTlVenE2OE5SdjFONGVuOCtsRUQyUE55NUs4UkQrTXN3V3kvYkYvdjRFaWxWYVlYa1ZIdGp0MXZyLytIYXhtU1lRVm51T2VFcWNuV04wcDJZTlpNMERjT3NHcDYyRmNvcHpYWnpZSGVlM2RsWUxTRk0xWnhUcFEzdTFOelJS",
  "Content-Type": "application/json"
}
```

Payload:

```json
{
  "packed": "I-*PHOdwlYFNwsR9eH62dJyy&Z",
  "unique_id": "f9e538b255c06209475e13d3f792cd0a14365c8ce417a9bef079762e9dfe0d60",
  "customer_ip": "93.115.127.129",
  "customer_key": "c0115490a57e0423165df3803ae2f106",
  "new_password": "22524172",
  "repeat_password": "22524172"
}
```

Response:

```json
{
  "result": {
    "code": 503074,
    "status": "Customer not found.",
    "request_number": "1779108565.487893.999850"
  }
}
```

HTTP status:

```text
501 Not Implemented
```

## Frontend/API Request That Triggered Final Step

Frontend SSO endpoint:

```text
POST https://app.sand.liracards.com/api/sso/lira/user/set-new-password
```

Payload:

```json
{
  "uniqueId": "41fae7b1f9dc89731cd1c819afbc9468574680c2e9ef1f12d86c27488b280ccd",
  "customerKey": "c0115490a57e0423165df3803ae2f106",
  "packed": "D0FT-5#bvh65c4PvlIK",
  "activeDatetime": "2026-05-18T12:35:36.028888Z",
  "timezone": "UTC",
  "newPassword": "22524172",
  "repeatPassword": "22524172"
}
```

SSO response:

```json
{
  "time": "2026-05-18T16:03:15.151479352",
  "code": 500,
  "message": "Internal Server Error",
  "body": null
}
```

Later structured logs confirmed the final Zeepay route was called:

```text
POST https://gateway.zeepay.com.tr/v2/Customer/ResetPassword/SetPassword
```

and Zeepay returned:

```json
{
  "result": {
    "code": 503074,
    "status": "Customer not found.",
    "request_number": "1779108565.487893.999850"
  }
}
```