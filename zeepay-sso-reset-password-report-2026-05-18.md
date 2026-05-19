# Reset password flow — Zeepay call log (sand)

**Source:** `logs/zeepay-service.log` on sand SSO  
**Date:** 2026-05-19  
**User:** national code `0010651861`, phone `9125264665`  
**Base URL:** `https://gateway.zeepay.com.tr`

---

## 1. Reset password by phone number

**Route**

```text
POST /v2/Customer/ResetPassword/ResetPasswordByPhoneNumber
```

**Full URL**

```text
https://gateway.zeepay.com.tr/v2/Customer/ResetPassword/ResetPasswordByPhoneNumber
```

**Time:** 2026-05-19 10:30:47

**Request body**

```json
{
  "id": "01f156350-5626-9eb0-8cfb-d60c44aa1cbc",
  "captcha": "hv7y4",
  "phone_country_code": "98",
  "phone_number": "9125264665",
  "customer_ip": "93.115.127.129"
}
```

**Response status**

```text
HTTP 200 OK
```

**Response body**

```json
{
  "result": {
    "code": 200,
    "status": "Success",
    "request_number": "1779174047.641410.189575"
  },
  "response": {
    "sms": {
      "receiver": "+98*******665",
      "reference": "01f156350-7690-c510-b48a-5693588d6d6f",
      "expires": "2026-05-19T07:03:47.650213Z",
      "timezone": "UTC"
    }
  }
}
```

---

## 2. Authenticate OTP

**Route**

```text
POST /v2/Customer/Authentication/Authentication
```

**Full URL**

```text
https://gateway.zeepay.com.tr/v2/Customer/Authentication/Authentication
```

**Time:** 2026-05-19 10:31:20

**Request body**

```json
{
  "receiver": "+989125264665",
  "code": "833739",
  "reference": "01f156350-7690-c510-b48a-5693588d6d6f",
  "customer_ip": "93.115.127.129"
}
```

**Response status**

```text
HTTP 200 OK
```

**Response body**

```json
{
  "result": {
    "code": 200,
    "status": "Success",
    "request_number": "1779174080.455826.648028"
  },
  "response": {
    "unique_id": "08a28dae6eb96554c8f451b65baab4cb293e93e68582dc97c045bd0e3bb3dcd4",
    "customer_key": "c0115490a57e0423165df3803ae2f106",
    "packed": "U5I@SG6*7Pcdnr-@7dXeB&FZ",
    "active_datetime": "2026-05-19T07:04:20.471710Z",
    "timezone": "UTC"
  }
}
```

---

## 3. Set new password

**Route**

```text
POST /v2/Customer/ResetPassword/SetPassword
```

**Full URL**

```text
https://gateway.zeepay.com.tr/v2/Customer/ResetPassword/SetPassword
```

**Time:** 2026-05-19 10:31:33

**Request body**

```json
{
  "packed": "U5I@SG6*7Pcdnr-@7dXeB&FZ",
  "unique_id": "08a28dae6eb96554c8f451b65baab4cb293e93e68582dc97c045bd0e3bb3dcd4",
  "customer_ip": "93.115.127.129",
  "customer_key": "c0115490a57e0423165df3803ae2f106",
  "new_password": "20304038",
  "repeat_password": "20304038"
}
```

**Response status**

```text
HTTP 501 Not Implemented
```

**Response body**

```json
{
  "result": {
    "code": 503074,
    "status": "Customer not found.",
    "request_number": "1779174094.054820.669866"
  }
}
```
